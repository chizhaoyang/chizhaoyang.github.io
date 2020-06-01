---
layout: archive
title: ""
permalink: /research/cooperative_navigation/
author_profile: true
redirect_from:
  - /research
---

{% include base_path %}

Cooperative Navigation using Inter-Vehicle Ranging and Magnetic Measurements
===
The objective of this research project is to enable groups of networked vehicles to perform robust relative and global navigation using inter-vehicle ranging and magnetic measurements. The presented approach contains two sequential steps: first, an algorithm called cooperative ranging localization, formulated as an Extended Kalman Filter (EKF), estimates each UAV’s relative pose inside the group using inter-vehicle ranging measurements; second, an algorithm named cooperative magnetic localization, formulated as a particle filter, estimates each UAV’s global pose through matching the group’s magnetic measurements to a given magnetic map.

The project contains three scenarios:

(1) UAV simulator with completed communication and simulated magnetic anomaly map. The completed communication means that each UAV is able to measure range and exchange information with each other UAV at every time step. The simulated magnetic anomaly map is generated using an upward continuation function with a Gaussian white noise.

<p align='center'>
    <img src="/images/completed_communication.png" alt="drawing" width="800"/>
    <img src="/images/simulated_map.png" alt="drawing" width="400"/>
</p>

(2) UAV simulator with Pairwise communication and the Earth's magnetic anomaly map. The pairwise communication means that each UAV is restricted to communicate and perform ranging measurements with only one other UAV at any point in time.

<p align='center'>
    <img src="/images/pairwise_communication.png" alt="drawing" width="800"/>
    <img src="/images/magnetic_map.png" alt="drawing" width="800"/>
    <img src="/images/simulator.png" alt="drawing" width="600"/>
</p>

(3) SMART robot experiments with limited ranging information and the magnetic intensity measurements. (In Process)

Results:

<p align='center'>
    <img src="/images/cooperative_result1.png" alt="drawing" width="800"/>
    <img src="/images/cooperative_result2.png" alt="drawing" width="800"/>
</p>

Related papers:

**Yang, Chizhao**, Jared Strader, Yu Gu, Alexander Hypes, Aaron Canciani, and Kevin Brink. "Cooperative UAV Navigation using Inter-Vehicle Ranging and Magnetic Anomaly Measurements." In *2018 AIAA Guidance, Navigation, and Control Conference*, p. 1595. 2018.

**Yang, Chizhao**, Jared Strader, Yu Gu, Aaron Canciani, and Kevin Brink, "Cooperative UAV Navigation using Magnetic Anomaly Measurements and Limited Inter-Vehicle Ranging Information." *Journal of Aerospace Information Systems*, In press.
