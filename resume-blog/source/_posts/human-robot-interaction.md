---
title: Human Robot Interaction(2021)
date: 2021-04-01 14:30:08
update: 2021-12-25 14:30:08
tags:
---
**This article records 3 human-robot-interaction demos implemented in 2021, which is mainly for the topic of my dissertation.**

# Human Collision Avoidance based on Global Skeleton Detection

The quick glance(left) is a demo for exploring collision avoidance between humans and manipulators through global skeleton detection.(The camera is not shown in the animation, but you can see it in the picture(right) of workspace setup.)

We use [Nuitrack](https://nuitrack.com/) to detect skeleton keypoints of human and then model these points as spheres which are given collision volume so that [Moveit!](https://moveit.ros.org/) can plan a trajectory to avoid collision. If there is any potential collision appearing in the trajectory, the manipulator will stop first and replan a new path so that it can get around the obstacles.

<div style="padding:5px; float:left">
<img src="https://raw.githubusercontent.com/ar-mine/ar-mine.github.io/images/human-collision-skeleton-experiment.gif" height=310px/>
</div>
<div style="padding:5px; float:right">
<img src="https://raw.githubusercontent.com/ar-mine/ar-mine.github.io/images/human-collision-skeleton-setup.jpg" height=310px/>
</div>
<!--more-->
The attached link is for the full video(without speeding up).
{% youtuber video Sf_YErWoBm4 %}
height: 310,
width: 620,
{% endyoutuber %}
<hr style="height:3px;background: #333"/>
<br/>

# GGCNN guided Grasping on the Plane and for Handover

<div style="padding:2px; float:left">
<img src="https://raw.githubusercontent.com/ar-mine/ar-mine.github.io/images/GGCNN%20plan%20pratical%20grasp.gif" width=300px/>
</div>
<div style="padding:2px; float:right;">
<img src="https://raw.githubusercontent.com/ar-mine/ar-mine.github.io/images/handover%20stable.gif" width=300px/>
</div>

The first quick glance is a demo grasping objects fixed on the plane and the second one shows a human-to-robot handover task which means that robot tries to grasp from human hand while avoiding to collide with people meanwhile. Both two demos are based on [GGCNN](https://github.com/dougsm/ggcnn), a light-weight network structure that can give pose candidates for grasping. 

The attached link is for the full video of two experiments(without speeding up).

{% youtuber video w83TNKI83qw %}
height: 310,
width: 620,
{% endyoutuber %}
<hr style="height:3px;background: #333"/>
<br/>

# PBVS tracking for marker and hand
<div style="padding:2px; float:left">
<img src="https://raw.githubusercontent.com/ar-mine/ar-mine.github.io/images/PBVS%20tracking%20for%20marker.gif" width=300px/>
</div>
<div style="padding:2px; float:right;">
<img src="https://raw.githubusercontent.com/ar-mine/ar-mine.github.io/images/PBVS-tracking-for-hand.gif" width=300px/>
</div>

These two demos are to implement servoing interface for UR3e robot based on (Position based Visual Servoing)PBVS instead of using Moveit. The first demo uses Acuro makers as target pose while the second one track hand which is processed by [BiSeNet](https://github.com/CoinCheung/BiSeNet). To use the network in my task, I train it with [LIP](https://arxiv.org/abs/1703.05446) and [Egohand](http://vision.soic.indiana.edu/projects/egohands/) dataset by myself.

The attached link is for the full video of two experiments(without speeding up).

{% youtuber video BBpfJdAknTI %}
height: 310,
width: 620,
{% endyoutuber %}

