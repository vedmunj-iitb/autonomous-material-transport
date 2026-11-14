# Autonomous material transport with a SLAM-based mobile robot

My Dual Degree Project (M.Tech. thesis) at IIT Bombay, July 2026 to present.

A TurtleBot 4 runs the trolley trips of a fan assembly line on its own, and a Gazebo copy of the
line lets several robots share those trips.

![The line in Gazebo](docs/overview.jpg)

## What I built

- The robot software on ROS 2 Jazzy, with Nav2 and SLAM Toolbox: state estimation, planning,
  control and actuation, on a TurtleBot 4 (Create 3 base, Raspberry Pi 4B, RPLIDAR A1M8)
- A lidar map of the line with its stations, and a startup that checks each stage before the robot
  moves
- A tuned Nav2 MPPI controller, retries when a station is missed, infrared docking and battery
  limits
- A web panel so lab staff can run the robot without a terminal
- A Gazebo simulation of the line in which three robots share the transport jobs

## Results

- 12 route trials scored from the robot's own logs: 100 of 112 station visits reached
- Fleets of 1 to 6 simulated robots: output rose from 21.9 to 47.9 fans an hour

![Top view of the simulated line](docs/topdown.jpg)

## Code

The code is private for now. Write to me if you would like to know more about the project.
