---
title: 'Motor-level N-MPC for cooperative active perception with multiple heterogeneous UAVs'
collection: publications
permalink: /publication/paper_7
excerpt: 'This letter introduces a cooperative control framework based on Nonlinear Model Predictive Control (NMPC) for solving an Active Information Acquisition problem (AIA) using a system of multiple multirotor UAVs equipped with onboard sensors. The observation task of the NMPC is a minimum-uncertainty pose estimation of a moving feature which is observed by the multi-UAV system, using a cooperative Kalman filter. The controller considers a full nonlinear model of the multirotors – including the motor-level actuation units and their real constraints in terms of maximum torque – and embeds the Kalman filter estimation uncertainty in its prediction. The framework allows and exploits heterogeneity in the actuation and sensing systems by considering a generic model of UAV – including both quadrotors and tilted-propeller multirotors – and a generic model of range-and-bearing sensor with arbitrary rate and field of view. The capability of the proposed framework to reduce the cooperative estimation uncertainty of a static or a moving feature, thus leading the system to optimal sensing configurations, is demonstrated through Gazebo simulations and real experiments. The software is provided open-source.'
date: 2022-04-01
venue: 'IEEE Robotics and Automation Letters'
venue_short: 'RA-L'
venue_type: 'Journal'
authors: 'Martin Jacquet, Max Kivits, Hemjyoti Das, Antonio Franchi'
topics: ['Optimal control & MPC', 'Perception & estimation']
paperurl: 'https://ieeexplore.ieee.org/abstract/document/9682606'
code: 'https://redmine.laas.fr/projects/active-perception-nmpc'
thumbnail: '/images/heterogeneous_NMPC.png'
citations: 26
scholar_url: 'https://scholar.google.com/citations?view_op=view_citation&hl=en&user=B1NyZ9IAAAAJ&pagesize=100&citation_for_view=B1NyZ9IAAAAJ:O3NaXMp0MMsC'
bibtex: |
  @article{jacquet2022motor,
    title     = {Motor-Level N-MPC for Cooperative Active Perception With Multiple Heterogeneous UAVs},
    author    = {Jacquet, Martin and Kivits, Max and Das, Hemjyoti and Franchi, Antonio},
    url       = {http://dx.doi.org/10.1109/LRA.2022.3143218},
    journal   = {IEEE Robotics and Automation Letters},
    volume    = {7},
    number    = {2},
    pages     = {2063–2070},
    publisher = {Institute of Electrical and Electronics Engineers (IEEE)},
    year      = {2022},
    ISSN      = {2377-3774}
  }
---
