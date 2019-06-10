cmake_minimum_required(VERSION 2.8.3)
project(wibotic_models)
# Load catkin and all dependencies required for this package
find_package(catkin REQUIRED COMPONENTS gazebo_ros)

catkin_package()

# Depend on system install of Gazebo
find_package(gazebo REQUIRED)

install(
  DIRECTORY 
    wibotic-git-models/models
    wibotic-git-models/meshes
    wibotic-git-models/materials 
    wibotic-git-models/urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)