---
title: "Nonlinear model predictive control for human-robot handover with application to the aerial case"
collection: publications
permalink: /publication/paper_8
excerpt: 'In this article, we consider the problem of delivering an object to a human coworker by means of an aerial robot (AR). To this aim, we present an ergonomics-aware Nonlinear Model Predictive Control (NMPC) designed to autonomously perform the handover. The method is general enough to be applied to any multi-rotor aerial vehicle (MRAV) with a minimal adaptation of the robot model. The formulation of the optimal control problem steers the AR toward a handover location by optimizing the human coworker ergonomics, which includes the predicted arm joint torques of the human. The motion task is expressed in a frame relative to the human, whose motion model is included in the equations of the NMPC. This allows the controller to promptly adapt to the human movements by predicting her future poses over the horizon. The control framework also accounts for the problem of maintaining visibility on the human coworker, while respecting both the actuation and state limits of the robot. Additionally, a safety barrier is embedded in the controller to avoid any risk of collision with the human partner. Realistic simulations are performed to validate the feasibility of the approach and the source code of the implementation is released open-source.'
date: 2022-10-23
venue: 'IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)'
paperurl: 'https://ieeexplore.ieee.org/abstract/document/9981045'
---
