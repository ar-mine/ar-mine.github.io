---
title: Human Robot Interaction(Recently)
date: 2022-01-27 11:47:52
tags:
---

# Slow Down or Stop by using Proximity Sensor

<br/>
<div style="padding:5px; float:left">
<img src="https://raw.githubusercontent.com/ar-mine/ar-mine.github.io/images/task1-real.gif" width=260px/>
</div>

According to the distance to collision, the robot can do some reactions like slowing down and even stop if it is close enough. To avoid the influence of the ray shadowed by itself, I code with [FCL](https://github.com/flexible-collision-library/fcl) and implement the visualization of collision and self-collision check between robot body and sensors' ray.

<br/>
<!--more-->
<hr style="height:3px;background: #333"/>
<br/>

# Collision Avoidance based on the Admittance Control
I model the distance to collision as force imposed on the end effector of robot arm and implement an admittance controller to make it avoid collision.
<div style="padding:5px; float:left">
<img src="https://raw.githubusercontent.com/ar-mine/ar-mine.github.io/images/task2-real.gif" height=165px/>
</div>
<div style="padding:5px; float:left">
<img src="https://raw.githubusercontent.com/ar-mine/ar-mine.github.io/images/task2-rviz.gif" height=165px/>
</div>

The attached player is for the full video for above two demos.

{% youtuber video -aYnKDmrGJ8 %}
height: 310,
width: 620,
{% endyoutuber %}