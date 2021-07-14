# Navigation_robot_Project

This projectj ast  of how a robot can be more intelligent about its movement than the random walk of  .This is done using Ros in ubuntu 16.04. and with robots from Turtlebot (https://emanual.robotis.com/docs/en/platform/turtlebot3/overview/).

1-Navigation Simulation:-

-Launch Simulation World

$ export TURTLEBOT3_MODEL=burger

$ roslaunch turtlebot3_gazebo turtlebot3_world.launch

![Screenshot from 2021-07-14 00-37-55](https://user-images.githubusercontent.com/86461558/125631660-61610655-3a62-494e-8c19-2d512c285eb9.png)


-Run Navigation Node

$ export TURTLEBOT3_MODEL=burger

$ roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml

-Estimate Initial Pose

1-Click the 2D Pose Estimate button in the RViz menu.

![2d_pose_button](https://user-images.githubusercontent.com/86461558/125630886-d752f373-6757-404a-a434-b661815bc6ed.png)


2-Click on the map where the actual robot is located and drag the large green arrow toward the direction where the robot is facing.

3-Repeat step 1 and 2 until the LDS sensor data is overlayed on the saved map.

4-Launch keyboard teleoperation node to precisely locate the robot on the map.

$ roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch

![Screenshot from 2021-07-14 06-53-22](https://user-images.githubusercontent.com/86461558/125632191-6f606707-e0ba-41c6-b047-dff8a568db81.png)


-Set Navigation Goal

1-Click the 2D Nav Goal button in the RViz menu.

![2d_nav_goal_button](https://user-images.githubusercontent.com/86461558/125630630-3ea0eb39-5310-4f2b-8afe-7ad4fb22fd59.png)

2-Click on the map to set the destination of the robot and drag the green arrow toward the direction where the robot will be facing.

![Screenshot from 2021-07-14 06-54-47](https://user-images.githubusercontent.com/86461558/125632367-c0b6a0b9-0c3b-4d17-972e-4bdc3f360b71.png)

