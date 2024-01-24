## Overview

Notes on ever expanding list of articles and projects that I want to work on and write about.

### article/blog ideas

- Shakey the robot, history of algos (A* etc), it's significance; gazebo/urdf for simulation - bring it to life

- CMU robot hall of fame: explore the different robots that were inducted and their history and significance

- ACDC Cloud Inference Evaluation Research Project writeup
    - Comparing the methodology and time evaluation of the MQTT based inference with TF Serving for inferencing self driving camera feed

- movie Hackers (1995). thoughts on it; specifically the times it was ridiculous and the times it actually referenced genuine hacker subculture (eg., books it referenced, "RISC-V is the future", etc)

- A quiet revolution in robotics (youtube: [Distinguished Colloquium: Vladlen Koltun, Sept 12, 2023 ](https://www.youtube.com/watch?v=K09erFsOnxA) and [MIT Robotics – Vladlen Koltun – A Quiet Revolution in Robotics Continued ](https://www.youtube.com/watch?v=vNFTcD3QMn0))
    - notes and thoughts; key ideas

- robot behaviours? can behaviour be encoded? 
    - explore current breakthroughs and seminal papers
        - (eg disney's new rl based robot character pipeline [How Disney Packed Big Emotion Into a Little Robot, IEEE Spectrum](https://spectrum.ieee.org/disney-robot), machine behaviour paper [Machine behaviour, Nature](https://www.nature.com/articles/s41586-019-1138-y) )
    - parallels from other sub fields

- Movies and series I love and why I love them; notes
    - Hirak Rajar Deshe
    - KungFu Hustle
    - Her
    - Halt and Catch Fire

- Demystify/explore common popular and useful ROS and robotics libraries (eg Nav2, ros_control, etc) 

### experiments

- Phone2proc [github](https://github.com/allenai/phone2proc) inspired open source (in lieu of the Apple Roomplan API etc) project for transforming your current environment setup into a simulation ready environment (to allow for training/evaluating simulations on your specific setup; trying to reduce sim2real gap)
    - use open source 3d semantic slam and other pieces

- data collection and training pipeline from robot simulations, to be used for Visual Action Models (VLA) models for robotics
    - ROS CI-CD devops pipeline at scale

- Control robotic arm with mobile phone 3d pose (position and orientation) using PWA; mobile pose calculated via camera video and IMU data, sent to robotic arm as input, mapping the 3d space coordinates from the mobile and the 3d space of the robot arm
    - extension of project done as RA at IGMR, RWTH Aachen.
    - replace the webXR pose api with open source slam models (AlvaAR project for eg. or ORB-SLAM3 wasm implementation)

- work on curation effort for the robotic worlds gazebo simulations and robotics datasets online visualisation;
    - simulations: curate publicly available gazebo simulation world environments and robot simulations
        - to be eventually used for quick testing with other ROS based libraries eg Nav2, SLAM libraries etc
    - robotics datasets: curate publicly available datasets and make it easy to browse the different data types and see easily what they consist of.
        - inspired by the RT-X project, but references/links to data sources separately (multiple can be put together and downloaded based on user's preference and need)

- VLA for robotics using small/tiny LLMs (eg mistral 7b etc) and fine tuning them for the specific tasks, replacing "heavier" models in current SOTA approaches

- QKD as secure transport layer for robotics; plugin into ROS workflow
    - modify open source implementations of QKD BB84 (using quantum simulations) 
    - should be compatible with real QKD hardware (if possible)

- ROS2 DDS deep dive

