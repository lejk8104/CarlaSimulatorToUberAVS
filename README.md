# CarlaSimulatorToUberAVS
this is autonomy sensor data visualization using XVIZ API
our vision
first. We make KITTI example (Uber XVIZ kitti example)
second. We make autonomy sensor data visualization system for Carla Simulator (Ford HMI)
finally. We make autonomy sensor data visualization system for DGIST autonomous Car

1. Convert to KITTI open dataset into XVIZ data
  1-1. convert to KITTI data into ROS bag file using "kitti2bag"
  link https://github.com/tomas789/kitti2bag
  1-2 create ROS-config using xviz-ros tool
  1-3 make GLB file, meta data using kitti.json , ros-xviz builder
  link https://github.com/uber/xviz/tree/master/examples/converters/ros

2. Convert to Carla Simulator data into XVIZ data 
  2-1. convert to Carla Simulator data into ROS bag file using "ROS bridge for CARLA simulator"
  link https://github.com/carla-simulator/ros-bridge
  2-2 create ROS-config using xviz-ros tool
  link https://github.com/uber/xviz/blob/master/docs/api-reference/ros/tools/xvizros-tool.md
  2-3. custom ROS-converter refer to "xviz-ros custom exmaple
  link https://github.com/uber/xviz/tree/master/examples/converters/ros-custom
  2-4. make GLB file, meta data using xviz bulider and xviz meta builder

