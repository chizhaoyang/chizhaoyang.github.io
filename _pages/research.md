---
layout: archive
title: ""
permalink: /research/
author_profile: true
redirect_from:
  - /research
---

{% include base_path %}
[NASA Sample Return Robot Centennial Challenge (Year 2016)](http://www.youtube.com/watch?v=ThKvmDHuXdU)
===
The main idea of NASA Sample Return Robot(SRR) Centennial Challenge was to encourage inovators to build fully-autonomous robots that can find, retrieve, and return samples in a large (~80,000m^2) outdoor environment without relying on Earth based technologies (e.g. GPS or magnetormeter). In 2016, the robot we built, named "Cataglyphis", completed the final SRR Challenge and won a $750,000 prize.

In this project, I contributed in two aspects:
1. Developed a Simultaneous Localization and Mapping (SLAM) algorithm as the localization system of Cataglyphis. The SLAM algorithm was built as a keyframe based factor graph structure. Lidar odometry was estimated  through matching two point cloud using Iterative Closest Point (ICP) algorithm with the inertial odometry estimate as initial guess. The inertial odometry was estimated based on the measurements from wheel encoder and gyroscope. To increase the robustness of the whole system, the intensity measurements from Lidar sensor were applied to evaluate the performances of the Lidar odometry and the inertial odometry. The factor graph was optimized using g2o algorithm when loop closure was detected.
2. Design a local map based collision avoidance system. While driving toward these waypoints, Cataglyphis generated a 2-D occupancy grid (named "hazard map") of detected obstacles relative to the robot using Lidar data. Additional obstacle detection was performed using random sample consensus (RANSAC) to find holes or small protrusions in the ground. Multiple predefined paths were evaluated using the hazard map, and the most effective one was adopted.

Related paper:

Gu, Yu, Jared Strader, **Chizhao Yang** et al. "Robot foraging: Autonomous sample return in a large outdoor environment." *IEEE Robotics & Automation Magazine* 25, no. 3 (2018): 93-101.

Video:

[![](http://img.youtube.com/vi/ThKvmDHuXdU/0.jpg)](http://www.youtube.com/watch?v=ThKvmDHuXdU "NASA Sample Return Robot Centennial Challenge (Year 2016)")
[![](http://img.youtube.com/vi/I5ILl1QPxr0/0.jpg)](http://www.youtube.com/watch?v=I5ILl1QPxr0 "2017 Robotic Easter Egg Hunt by Cataglyphis")

[Precision Pollination Robot](http://www.youtube.com/watch?v=66isrgth7-Q)
===
The objective for this project is to design a prototype pollinator robot, named BrambleBee, and perform proof-of-concept demonstrations of its effectiveness for brambles (i.e. blackberry and raspberry) pollination in a greenhouse environment. During the project, we developed the ability to precisely locate, evaluate, interact, and manipulate small and delicate plant structures within unstructured, low-dynamic, and GPS-challenged environments, which is an enabling technology for supporting future integrated crop management systems.

My jobs in this project:

Designed and developed the localization system for the pollinator robot, BrambleBee. The system is able to provide low-drift and high update rate (i.e., 50 Hz) pose estimates and to update the map of the environment. The system utilize three primary information sources: 3D point cloud scans provided by the LiDAR, the acceleration and angular velocity measurements provide by the IMU and the velocity measured by wheel odometry.

Related papers:

**Yang, Chizhao**, Ryan Watson, Jason Gross, Yu Gu, "Localization Algorithm Design and Evaluation for an Autonomous Pollination Robot," *Proceedings of the 32nd International Technical Meeting of the Satellite Division of The Institute of Navigation (ION GNSS+ 2019)*, pp. 2702-2710, 2019.

Strader, Jared, Jennifer Nguyen, **Chizhao Yang** et al. "Flower Interaction Subsystem for a Precision Pollination Robot." In *2019 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)*, pp. 5534-5541. IEEE, 2019.

Ohi, Nicholas, Kyle Lassak, **Chizhao Yang** et al. "Design of an autonomous precision pollination robot." In *2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)*, pp. 7711-7718. IEEE, 2018.

Image:

<p align='center'>
    <img src="/images/farm_slam.png" alt="drawing" width="800"/>
</p>

Videos:

[![](http://img.youtube.com/vi/66isrgth7-Q/0.jpg)](http://www.youtube.com/watch?v=66isrgth7-Q "BrambleBee Greenhouse Pollination Experiment with QR Flowers")
[![](http://img.youtube.com/vi/ZbgtP9CHycA/0.jpg)](http://www.youtube.com/watch?v=ZbgtP9CHycA "BrambleBee Robot Pollinating a High-Fidelity Artificial Plant")


Cooperative Navigation using Inter-Vehicle Ranging and Magnetic Measurements
===
The objective of this research project is to enable groups of networked vehicles to perform robust relative and global navigation using inter-vehicle ranging and magnetic measurements.

The project contains three subprojects:

1. UAV simulator with completed communication and the Earth's magnetic anomaly measurements.


2. UAV simulator with limited communication and the Earth's magnetic anomaly measurements.


3. SMART robot experiments with limited ranging information and the magnetic intensity measurements.

Related papers:

**Yang, Chizhao**, Jared Strader, Yu Gu, Alexander Hypes, Aaron Canciani, and Kevin Brink. "Cooperative UAV Navigation using Inter-Vehicle Ranging and Magnetic Anomaly Measurements." In *2018 AIAA Guidance, Navigation, and Control Conference*, p. 1595. 2018.

**Yang, Chizhao**, Jared Strader, Yu Gu, Aaron Canciani, and Kevin Brink, "Cooperative UAV Navigation using Magnetic Anomaly Measurements and Limited Inter-Vehicle Ranging Information." *Journal of Aerospace Information Systems*, in press.

Applying Autonomous Mobile Robots on Human-Robot Collaboration and Safety In Smart Warehouses
===

Path Planning
===
