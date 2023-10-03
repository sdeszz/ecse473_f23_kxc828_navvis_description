# ecse473_f23_kxc828_navvis_description
## Overview
This ROS package, `navvis`, provides functionalities to launch a robot simulation and visualize robot and sensor data in Rviz. You can utilize the provided launch files to get started with the simulation, and it allows you to visualize specific robot movements and sensor readings using ROS bag files.

## Prerequisites

- **ROS**: Ensure you have the [Robot Operating System (ROS)](http://wiki.ros.org/ROS/Installation) installed and configured.
Install the URDF utilities
sudo apt install liburdfdom-dev liburdfdom-tools ros-<ros_version>-urdfdom-py

Install the joint_state_publisher_gui package if Melodic or newer
sudo apt install ros-<ros_version>-joint-state-publisher-gui

Dependencies: Ensure all dependencies are installed:
rosdep install --from-paths src --ignore-src -r -y

Build Workspace: Make sure to build your workspace:
catkin_make
source devel/setup.bash

Usage
Launching the Robot Simulation
To launch the robot simulation, navigate to your workspace and use the following roslaunch command:
roslaunch navvis_description display.launch use_xacro:=true &
