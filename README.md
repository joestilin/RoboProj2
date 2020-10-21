# RoboProj2
Udacity Robotics Software Engineer Nanodegree Project #2. 

A simulted differential drive robot with camera and lidar sensors chases a white ball in a Gazebo world. A ```drive_bot``` ROS node 
requests linear and angular velocities for a differential drive from a ```process_image``` ROS node. 

## Dependencies

ROS: Install Robot Operating System (ROS) by following these instructions: http://wiki.ros.org/Installation
   * Follow the instructions for a Destop-Full Install, which will include rviz and other packages required by this repository.


Gazebo: Follow the instructions for your environment at http://gazebosim.org/tutorials?cat=install

Ubuntu one line installation:
```bash
$ curl -sSL http://get.gazebosim.org | sh
```

## Installation

Step 1:
Clone the repository into your workspace
```bash
$ git clone https://www.github.com/joestilin/RoboProj2
```

Step 2:
Initialize a catkin workspace inside src
```bash
$ cd /RoboProj2/catkin_ws/src
$ catkin_init_workspace
```
Step 3:
Move up to the catkin workspace root, build the package, and source the environment
```bash
$ cd ..
$ catkin_make
$ source devel/setup.bash
```

# Usage

Launch ```world.launch```
```bash
$ cd /RoboProj2/catkin_ws
$ roslaunch my_robot world.launch
```

Open a new terminal and launch ```ball_chaser.launch```
```bash
$ cd /RoboProj2/catkin_ws
$ source devel/setup.bash
$ roslaunch ball_chaser ball_chaser.launch
```

The robot steers left, right or straight depending on where the white ball is in the camera field of view!

Attributes:
XR wheel .dae file sourced from 3D Warehouse:
https://3dwarehouse.sketchup.com/model/bcdc810b52c8a430e4e346ee2650d150/XR-Wheels?tab=general
