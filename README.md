# WiBotic Systems in Gazebo Demo
This repository is meant to belong to a colcon workspace.
It has been tested with AWS RoboMaker

## To get started:
1. Create a new AWS RoboMaker development environment
2. Setup the environment structure with `mkdir -p simulation_ws/src && cd  simulation_ws/src` or navigate to your `src` directory if it already exists
3. Clone the contents of this repository into the `src` directory
4. Build and bundle the workspace using colcon with `colcon build && colcon bundle`. This will take several minutes
5. The simulation bundle `simulation_ws/bundle/output.tar` can now be uploaded to your S3 source bucket and run in a simulation job
6. The intended launch package of this bundle is `wibotic_gazebo` with the launch file `example.launch`
