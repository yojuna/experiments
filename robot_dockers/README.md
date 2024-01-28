# ROS Gazebo dockers workflow

Trying to run AWS robotics bookstore world with ROS gazebo docker based development workflow

```
cd robot_dockers/ros_gazebo_dockers
```

```
# Start the dev container
docker compose up dev

# Open as many interactive shells as you want to the container
docker compose exec -it dev bash
```

## AWS Bookstore example

get the repo:
    - has been added as submodule and should be available if recursively cloned, otherwise
```
git clone https://github.com/aws-robotics/aws-robomaker-bookstore-world.git
```

### First time after fork

- needed to switch to ros2 branch

Inside a new interactive shell, (alongside the dev container running in other terminal)

go inside the models repo:
```
cd src/aws-robomaker-bookstore-world/
```

```
# Run world in Only Gazebo without ROS
export GAZEBO_MODEL_PATH=`pwd`/models
gazebo worlds/bookstore.world
```

```
# ROS launch with gazebo

# build for ROS
rosdep install --from-paths . --ignore-src -r -y
colcon build

# run in ROS
source install/setup.sh
ros2 launch aws_robomaker_bookstore_world view_bookstore.launch.py
```

Expected output/workflow example
```
nemo@homelab:~/code/repos/experiments/robot_dockers/ros_gazebo_dockers$ docker compose exec -it dev bash
Sourced ROS 2 humble
Sourced TurtleBot3 base workspace
devuser@homelab:/overlay_ws$ cd src/aws-robomaker-bookstore-world/
devuser@homelab:/overlay_ws/src/aws-robomaker-bookstore-world$ rosdep install --from-paths . --ignore-src -r -y
#All required rosdeps installed successfully
devuser@homelab:/overlay_ws/src/aws-robomaker-bookstore-world$ colcon build
Starting >>> aws_robomaker_bookstore_world
Finished <<< aws_robomaker_bookstore_world [3.44s]                  

Summary: 1 package finished [4.42s]
devuser@homelab:/overlay_ws/src/aws-robomaker-bookstore-world$ source install/setup.sh

devuser@homelab:/overlay_ws/src/aws-robomaker-bookstore-world$ ros2 launch aws_robomaker_bookstore_world bookstore.launch.py

# For GUI

devuser@homelab:/overlay_ws/src/aws-robomaker-bookstore-world$ ros2 launch aws_robomaker_bookstore_world view_bookstore.launch.py
```
^^ note: ros launch currently causes gz to fail

### issues:

#### docker view bookstore gazebo failing
[gzclient-2] gzclient: /usr/include/boost/smart_ptr/shared_ptr.hpp:728: typename boost::detail::sp_member_access<T>::type boost::shared_ptr<T>::operator->() const [with T = gazebo::rendering::Camera; typename boost::detail::sp_member_access<T>::type = gazebo::rendering::Camera*]: Assertion `px != 0' failed.
[ERROR] [gzclient-2]: process has died [pid 1063, exit code -6, cmd 'gzclient'].

