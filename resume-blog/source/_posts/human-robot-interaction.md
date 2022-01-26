---
title: Human Robot Interaction(2021)
date: 2021-04-01 14:30:08
update: 2021-12-25 14:30:08
tags:
---
**This article records 3 human-robot-interaction demos implemented in 2021, which is mainly for the topic of my dissertation.**

# Human Collision Avoidance based on Global Skeleton Detection

The left quick glance is a demo for exploring collision avoidance between humans and manipulators through global skeleton detection.(The camera is not shown in the quick glance, but you can see it in the picture of workspace setup.)

We use Nuitrack to detect skeleton keypoints of human and then model these points to balls which are given collision volume so that Moveit! can plan a trajectory to avoid collision. If there is any potential collision appearing in the trajectory, the manipulator will stop first and replanning a new path then.

<div style="padding:5px; float:left">
<img src="https://raw.githubusercontent.com/ar-mine/ar-mine.github.io/images/human-collision-skeleton-experiment.gif" height=310px/>
</div>
<div style="padding:5px; float:right">
<img src="https://raw.githubusercontent.com/ar-mine/ar-mine.github.io/images/human-collision-skeleton-setup.jpg" height=310px/>
</div>
<!--more-->
The attached player is for the full video.
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

The first quick glance is a demo grasping objects fixed on the plane and the second one is a handover which means that robot tries to grasp from human hand while avoiding to collide with people meanwhile. Both two demos are based on GGCNN, a light-weight network structure that can give best poses for grasping. 

The attached player is for the full video.

{% youtuber video w83TNKI83qw %}
height: 310,
width: 620,
{% endyoutuber %}
<hr style="height:3px;background: #333"/>
<br/>

# PBVS tracking for marker and hand
The attached player is for the full video.

{% youtuber video BBpfJdAknTI %}
height: 310,
width: 620,
{% endyoutuber %}

