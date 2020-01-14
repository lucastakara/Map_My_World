# Map my World Project
---

## Introduction
-----

The goal of this project is a implementation of the Real-Time Appearance Based Mapping (RTAB-Map) algorithm in ROS (Robot Operational System) to perform SLAM in a simulated environment.
 
![Gazebo](https://github.com/lucastakara/Map_my_world/blob/master/src/images/graph.png?raw=true)

## Concepts
---
The following concepts will be explored in this project:
- Gazebo models and world-building 
- Gazebo plugins
- URDF6
- XML
- ROS essentials: Publishers, Subscribers and Services
- C++
- ROS RTABMAP package

## Getting Started
----
The following items are required in order to visualize and create the project:
 
#### Installation Instructions:

#### Prerequisites / Dependencies 

- Gazebo >= 7.0

- ROS Kinetic

- gcc/g++ >= 5.4

- Linux: gcc / g++ is installed by default on most Linux distros

- [Linux Ubuntu 16.04.6 LTS (Xenial Xerus)](http://releases.ubuntu.com/16.04/)
- [Gazebo](http://gazebosim.org/tutorials?tut=install_ubuntu&cat=install) 
- [Robot Operating System](http://wiki.ros.org/kinetic/Installation/Ubuntu) (ROS)
-

Once these components are installed, you need to create a Catkin Workspace:


- `$ mkdir -p catkin_ws/src`

- `$ cd catkin_ws/src`

- `$ catkin_init_workspace`

Download/clone the repository and copy the "my_robot", directory in the src directory:

- `$ git clone https://github.com/lucastakara/Map_my_world`


`Then, navigate up to the top-level catkin workspace directory and build the executables:

- `cd ..`
- `catkin_make` 

Next, you can open Gazebo with the robot in it:

- `$ source devel/setup.bash`

- `$ roslaunch my_robot world.launch`

- `$ roslaunch my_robot mapping.launch`

This will initialize all the nodes. 

To operate the robot via the keyboard, open a second terminal, navigate to the root level directory and execute:

- `$ source devel/setup.bash`
- `$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py`


