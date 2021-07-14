# Navigation_robot_Project

This projectj ast  of how a robot can be more intelligent about its movement than the random walk of  .This is done using Ros in ubuntu 16.04. and with robots from Turtlebot (https://emanual.robotis.com/docs/en/platform/turtlebot3/overview/).

1-Navigation Simulation:-

-Launch Simulation World

$ export TURTLEBOT3_MODEL=burger

$ roslaunch turtlebot3_gazebo turtlebot3_world.launch

-Run Navigation Node

$ export TURTLEBOT3_MODEL=burger

$ roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml

-Estimate Initial Pose

1-Click the 2D Pose Estimate button in the RViz menu.

2-Click on the map where the actual robot is located and drag the large green arrow toward the direction where the robot is facing.

3-Repeat step 1 and 2 until the LDS sensor data is overlayed on the saved map.

4-Launch keyboard teleoperation node to precisely locate the robot on the map.

$ roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch

-Set Navigation Goal

1-Click the 2D Nav Goal button in the RViz menu.

2-Click on the map to set the destination of the robot and drag the green arrow toward the direction where the robot will be facing
