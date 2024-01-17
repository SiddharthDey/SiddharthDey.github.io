---
layout: page
title: Particle Filter SLAM
---

Used Particle Filter to perform SLAM for a LiDAR-equipped wheeled robot 

- The data for the robot came from the sensors mounted on it, including a Hokuyo UTM-30LX LiDAR sensor and a Kinect RGB-D camera

- The robot's trajectory (2D pose and angular orientation at each time stamp) and the static map in the form of an occupancy grid map were estimated using the particle filter algorithm

- RGB values from the camera were used to produce a 2D color/texture map of the floor surface based on the occupancy grid map generated previously

You can find the project report here [[Link]](https://drive.google.com/file/d/1AQXA0KcFs-B63mxKaA_FmfN-TuLewVeh/view?usp=sharing)

{% include embed.html url="https://drive.google.com/file/d/1eCCOQhDZHPj4QzMRr-wym41U68jymv10/preview" %}
<p style="text-align: center;">
Visualization of trajectory and occupany grid generation using Particle Filter
</p>
<!-- {% include embed.html url="https://drive.google.com/file/d/1eCCOQhDZHPj4QzMRr-wym41U68jymv10/view?usp=sharing" %} -->
<!-- <iframe src="https://drive.google.com/file/d/1eCCOQhDZHPj4QzMRr-wym41U68jymv10/view?usp=sharing" width="640" height="480"></iframe> -->











