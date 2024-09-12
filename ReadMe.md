# IDMP-Framework - Interactive Distance Field Mapping and Planning to Enable Human-Robot Collaboration

This repository combines all necessary repositories to run the IDMP-Framework.

 * Main repository for IDMP, implementing a gaussian process based distance and gradient field algorithm.
    * [Project Page](https://uts-ri.github.io/IDMP/)
    * [Paper](https://arxiv.org/abs/2403.09988v1)
    * [Video](https://www.youtube.com/watch?v=NpbDjCqXyrs)

 * Repository for RMP, riemannian motion policies using the IDMP distance and gradient field.
    * [Project Page](https://uts-ri.github.io/IDMP/)
    * [Paper](https://arxiv.org/abs/2403.09988v1)
    * [Video](https://www.youtube.com/watch?v=NpbDjCqXyrs)
 * Universal Robots ROS Driver
 * Universal Robots and Robotiq HandE Models


 This codebase is implemented using ROS Noetic in both C++14 and Python 3.8.10.

 ## Description

 

## Dependencies

- Python3
- C++14
- ROS Noetic
- Eigen
- OpenMP (for multithreading. optional but strongly recommended)
- sensor-filters (`sudo apt install ros-noetic-sensor-filters`)
- point-cloud2-filters (`sudo apt install ros-noetic-point-cloud2-filters`)
- robot-body-filter (optional for removing the robot from the pointcloud. `sudo apt install ros-noetic-point-cloud2-filters`)
- Camera specific ros driver
    - [Azure kinect](https://github.com/microsoft/Azure_Kinect_ROS_Driver)
    - [Intel Realsense](https://github.com/IntelRealSense/realsense-ros)
    - [ZED 2i](https://github.com/stereolabs/zed-ros-wrapper)
- For Python tools:
    - numpy
    - OpenCV 4.9.0
    - Open3D (for evaluation only)
- [ur_rtde v.1.5.8 ](https://gitlab.com/sdurobotics/ur_rtde.git)
- ur_describtion (`sudo apt install ros-noetic-ur_description`)

## Installation

The Framework is provided as multiple catkin packages

- clone the package into the src folder of your workspace
- run a `catkin build`
- resource your workspace