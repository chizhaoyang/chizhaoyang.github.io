---
layout: archive
title: ""
permalink: /research/
author_profile: true
redirect_from:
  - /research
---

{% include base_path %}
NASA Sample Return Robot Centennial Challenge (Year 2016)
------
The main idea of NASA Sample Return Robot(SRR) Centennial Challenge was to encourage inovators to build fully-autonomous robots that can find, retrieve, and return samples in a large (~80,000m^2) outdoor environment without relying on Earth based technologies (e.g. GPS or magnetormeter). In 2016, the robot we built, named "Cataglyphis", completed the final SRR Challenge and won a $750,000 prize.

In this project, I contributed in two aspects:
1. Developed a Simultaneous Localization and Mapping (SLAM) algorithm as the localization system of Cataglyphis. The SLAM algorithm was built as a keyframe based factor graph structure. Lidar odometry was estimated  through matching two point cloud using Iterative Closest Point (ICP) algorithm with the inertial odometry estimate as initial guess. The inertial odometry was estimated based on the measurements from wheel encoder and gyroscope. To increase the robustness of the whole system, the intensity measurements from Lidar sensor were applied to evaluate the performances of the Lidar odometry and the inertial odometry. The factor graph was optimized using g2o algorithm when loop closure was detected.
2. Design a local map based collision avoidance system. While driving toward these waypoints, Cataglyphis generated a 2-D occupancy grid (named "hazard map") of detected obstacles relative to the robot using Lidar data. Additional obstacle detection was performed using random sample consensus (RANSAC) to find holes or small protrusions in the ground. Multiple predefined paths were evaluated using the hazard map, and the most effective one was adopted.

Related paper:
Gu, Yu, Jared Strader, **Chizhao Yang** et al. "Robot foraging: Autonomous sample return in a large outdoor environment." *IEEE Robotics & Automation Magazine* 25, no. 3 (2018): 93-101.

Video:

[![center](http://img.youtube.com/vi/ThKvmDHuXdU/0.jpg)](http://www.youtube.com/watch?v=ThKvmDHuXdU "NASA Sample Return Robot Centennial Challenge (Year 2016)")

Precision Pollination Robot
------

Cooperative UAV Navigation using Inter-Vehicle Ranging and Magnetic Measurements
------

Applying Autonomous Mobile Robots on Human-Robot Collaboration and Safety In Smart Warehouses
------

Path Planning
------
