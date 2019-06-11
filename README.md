# WiBotic Systems in Gazebo Demo
This repository is meant to belong to a colcon workspace.
It has been tested with AWS RoboMaker

## To get started:
1. Create a new AWS RoboMaker development environment
2. Run `sudo apt install ros-kinetic-gazebo-ros protobuf-compiler` to install the required build tools
3. Setup the environment structure with `mkdir -p simulation_ws/src && cd  simulation_ws/src` or navigate to your `src` directory if it already exists
4. Clone the contents of this repository into the `src` directory
5. Build and bundle the workspace using colcon with `colcon build && colcon bundle`. This will take several minutes
6. The simulation bundle `simulation_ws/bundle/output.tar` can now be uploaded to your S3 source bucket and run in a simulation job
7. The intended launch package of this bundle is `wibotic_gazebo` with the launch file `example.launch`
