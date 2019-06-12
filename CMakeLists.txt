cmake_minimum_required(VERSION 2.8.3)
project(aiut_nao)

## Compile as C++11, supported in ROS Kinetic and newer
add_compile_options(-std=c++11)

## Find catkin macros and libraries
## if COMPONENTS list like find_package(catkin REQUIRED COMPONENTS xyz)
## is used, also find other catkin packages
find_package(catkin REQUIRED COMPONENTS
  controller_manager
  gazebo_ros
  gazebo_ros_control
  sensor_msgs
  std_msgs
  urdf
)

catkin_package(
)
include_directories(
${PROJECT_SOURCE_DIR}/include/${PROJECT_NAME}
${catkin_INCLUDE_DIRS}
)

