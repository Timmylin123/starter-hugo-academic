---
title: Turtlebot Tag
date: 2022-10-06T17:02:22.974Z
draft: false
featured: false
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
In this project, we have two turtlebots (a chaser and a runner) playing tag. The runner moves in random directions and maintains that direction for a period of time. The chaser uses a path prediction algorithm to estimate where the runner will be, and catch it at that future location. The chaser achieves this by storing a history of the runner's locations, and uses statistical extrapolation algorithms to predict the path that the runner may be taking. Then, the chaser uses proportional control to move towards the predicted coordinate of the runner. Once the chaser tags the runner with its bumper sensor, the chaser will stop.

T﻿his project is collectively done by Ting-Han Lin, Evan Wu, Sam Shatzkin, and Diego Viveros (who were all students in the Introduction to Robotics class). Our project is interesting because it can use path prediction model to predict the future path of the runner much more accurately and can let the chaser tag the runner even when the chaser is operating at a lower speed than the runner.