# Autonomous_Mobile_Robot
## Descreption 
This autonomous mobile robot design was built using the Unified Robot Description Format (URDF) and it utilizes a skid steer drive system.

To facilitate mapping and navigation, I implemented the gmapping package, which employs laser-based SLAM (Simultaneous Localization and Mapping) techniques to generate a 2D occupancy grid map.

For accurate localization in a 2D environment, the robot employs AMCL, a probabilistic localization system.

Furthermore, the robot's navigation capabilities are powered by a comprehensive navigation stack. This stack integrates data from odometry, sensor feeds, and a designated goal pose. It then generates safe velocity commands, which are subsequently transmitted to the mobile base via the move_base package.

## Run robot in gazebo
```
roslaunch okasha_gazebo okasha_gazebo.launch
```
