---
title: "Machine Learning Algorithms for Structural Health Monitoring"
collection: projects
permalink: /projects/MLforSHM
excerpt: 'This work is about using ML algorithms to try and identify the level of damage sustained by a structure soon after the occurrence of a natural calamity.'
---

{% include base_path %}

[Github Code Repository link](https://github.com/SiddharthSaravanan/MLforSHM)
<br />
[Download Project Report](http://SiddharthSaravanan.github.io/files/MLforSHMreport.pdf)

The objective of this project is to use Machine Learning algorithms to determine the structural health of a building. More preciesely, the objective was to take noisy accelerometer data from accelerometers placed on two adjacent floors and be accurately predict the status of the building. The status of the building can be one of 3 classes, Immediate Occupancy (IO), Life Safety (LS) or Collapse Prevention (CP). The status of the building is therefore represented as a 1-dimensional array of size 3 which uses one-hot encoding. We used ML algoithms to take 2 noisy accelerometer readings and output a 1D array of size 3 which accurately represents the structural health of the structure.
