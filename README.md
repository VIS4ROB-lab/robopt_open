# Robotic Optimization (ROBOPT) Library #
Package to simplify implementation of optimization problems in Ceres commonly used in robotics.

## Installation  
In order to install RobOpt, follow these steps. First, create a catkin workspace:
```
$ mkdir -p catkin_ws/src
$ cd catkin_ws
```
Set-up the workspace:
```
$ catkin init
$ catkin config --extend /opt/ros/melodic
$ catkin config --cmake-args -DCMAKE_BUILD_TYPE=Release
$ catkin config --merge-devel
```

Clone the dependencies:
```
$ cd ~/catkin_ws/src
$ wstool init
$ wstool merge robopt_open/dependencies_ssh.rosinstall # To clone with https: robopt_open/dependencies_https.rosinstall
$ wstool up -j8
```  

Finally, build the package:
```
$ cd ~/catkin_ws
$ catkin build robopt_open
```  
