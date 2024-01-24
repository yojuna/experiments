### article/blog ideas

- Shakey the robot, history of algos (A* etc), it's significance; gazebo/urdf for simulation - bring it to life

- CMU robot hall of fame: explore the different robots that were inducted and their history and significance

- ACDC Cloud Inference Evaluation Research Project writeup
    - Comparing the methodology and time evaluation of the MQTT based inference with TF Serving for inferencing self driving camera feed

- movie Hackers (1995). thoughts on it; specifically the times it was ridiculous and the times it actually referenced genuine hacker subculture (eg., books it referenced, RISC-V is the future, etc)




### experiments

- Phone2proc [github](https://github.com/allenai/phone2proc) inspired open source (in lieu of the Apple Roomplan API etc) project for transforming your current environment setup into a simulation ready environment (to allow for training/evaluating simulations on your specific setup; trying to reduce sim2real gap)
    - use open source 3d semantic slam and other pieces

- data collection and training pipeline from robot simulations, to be used for Visual Action Models (VLA) models for robotics

- Control robotic arm with mobile phone 3d pose (position and orientation) using PWA; mobile pose calculated via camera video and IMU data, sent to robotic arm as input, mapping the 3d space coordinates from the mobile and the 3d space of the robot arm
    - extension of project done as RA at IGMR, RWTH Aachen.
    - replace the webXR pose api with open source slam models (AlvaAR project for eg. or ORB-SLAM3 wasm implementation)
