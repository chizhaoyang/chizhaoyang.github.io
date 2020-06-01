---
layout: archive
title: ""
permalink: /research/pollination/
author_profile: true
redirect_from:
  - /research
---

{% include base_path %}

Precision Pollination Robot
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
