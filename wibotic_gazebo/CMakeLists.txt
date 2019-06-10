cmake_minimum_required(VERSION 2.8.3)
project(wibotic_gazebo)
find_package(catkin REQUIRED)
catkin_package()

install(
  DIRECTORY launch worlds robots 
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)