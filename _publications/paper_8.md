---
title: 'Nonlinear model predictive control for human-robot handover with application to the aerial case'
collection: publications
selected: true
permalink: /publication/paper_8
excerpt: 'In this article, we consider the problem of delivering an object to a human coworker by means of an aerial robot (AR). To this aim, we present an ergonomics-aware Nonlinear Model Predictive Control (NMPC) designed to autonomously perform the handover. The method is general enough to be applied to any multi-rotor aerial vehicle (MRAV) with a minimal adaptation of the robot model. The formulation of the optimal control problem steers the AR toward a handover location by optimizing the human coworker ergonomics, which includes the predicted arm joint torques of the human. The motion task is expressed in a frame relative to the human, whose motion model is included in the equations of the NMPC. This allows the controller to promptly adapt to the human movements by predicting her future poses over the horizon. The control framework also accounts for the problem of maintaining visibility on the human coworker, while respecting both the actuation and state limits of the robot. Additionally, a safety barrier is embedded in the controller to avoid any risk of collision with the human partner. Realistic simulations are performed to validate the feasibility of the approach and the source code of the implementation is released open-source.'
date: 2022-10-23
venue: 'IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)'
venue_short: 'IROS'
venue_type: 'Conference'
authors: 'Gianluca Corsini, Martin Jacquet, Hemjyoti Das, Amr Afifi, Daniel Sidobre, Antonio Franchi'
topics: ['Optimal control & MPC', 'Human-robot interaction']
paperurl: 'https://ieeexplore.ieee.org/abstract/document/9981045'
code: 'https://redmine.laas.fr/projects/nmpc-handover'
thumbnail: '/images/physical_interaction.png'
citations: 26
scholar_url: 'https://scholar.google.com/citations?view_op=view_citation&hl=en&user=B1NyZ9IAAAAJ&pagesize=100&citation_for_view=B1NyZ9IAAAAJ:ns9cj8rnVeAC'
bibtex: |
  @inproceedings{corsini2022nonlinear,
    title     = {Nonlinear Model Predictive Control for Human-Robot Handover with Application to the Aerial Case},
    author    = {Corsini, Gianluca and Jacquet, Martin and Das, Hemjyoti and Afifi, Amr and Sidobre, Daniel and Franchi, Antonio},
    url       = {http://dx.doi.org/10.1109/IROS47612.2022.9981045},
    booktitle = {2022 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)},
    pages     = {7597–7604},
    publisher = {IEEE},
    year      = {2022}
  }
---
