# ROS2 Nodes

## lidar_node
- Located in: `my_robot/my_robot/lidar_node.py`
- Function: Reads data from the RPLIDAR A1 and publishes it as a ROS2 LaserScan message.
- Publishes: `/scan` (sensor_msgs/LaserScan)
- Subscribes: None

## slam_node
- Located in: `my_robot/my_robot/slam_node.py`
- Function: Performs SLAM using LIDAR data.
- Publishes: `/map` (nav_msgs/OccupancyGrid)
- Subscribes: `/scan`
