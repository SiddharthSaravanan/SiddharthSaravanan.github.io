---
title: "Composition and Rendering of Bharatanatyam Performance"
collection: projects
permalink: /projects/BharatnatyamAR
excerpt: 'This work is about using fewbb'
---

{% include base_path %}

[Github Code Repository link](https://github.com/SiddharthSaravanan/BharatanatyamAR)
<br />
[Project Report](https://www.researchgate.net/publication/351559537_Composition_and_Rendering_of_Bharatanatyam_Performance_in_Augmented_Reality)


The objective of this project was to write a program using [Blender's](https://www.blender.org/) [Python API](https://docs.blender.org/api/current/index.html) That is capable of taking a list of 30-dimenaional vectors and creating an animation of a dancer. Or simply put, going from this:
```
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
1 -1 2 0 2 -1 3 -1 -1 -1 3 0 1 1 2 1 1 1 0 2 2 0 0 0 -3 1 1 0 0 0
2 1 2 0 2 -1 3 -1 1 1 3 0 1 1 2 1 0 0 0 0 0 1 0 0 0 1 1 0 0 0
2 1 2 0 2 -1 3 -1 1 1 6 4 -2 0 2 0 0 0 0 0 0 1 0 0 0 1 1 0 0 0
2 1 2 1 2 0 3 0 0 0 0 2 -1 1 3 -1 0 0 0 0 0 0 0 0 0 0 1 0 0 0
1 -1 2 -2 2 0 2 0 0 0 0 2 -1 1 3 -1 0 0 0 0 0 0 0 0 0 0 1 0 0 0
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 
```

To this:

![Alt Text](https://media.giphy.com/media/mPgCNQh8b4qVl6EhKk/giphy.gif?cid=790b7611fc09703cd5ccb5306c7d03e060e8193d101e2c52&rid=giphy.gif&ct=g)

#Codification of a Bharathnatyam Pose

The Codification of a pose in Bharathanatyam into a 30-dimensional vector was done by professor Sangeeta Jadhav, Goa University (2018). In her work, posititions of different parts of the body are represented by different integers within the 30-dimensional vector as shown below:


>Position of Head : 1 and 2,<br />
>Position of Right Hand : 3 to 10,<br />
>Position of Left Hand : 11 to 18,<br />
>Waist position : 19 and 20,<br />
>Right Leg position : 21 to 25,<br />
>Left Leg position : 26 to 30.<br />




talk about thesis
Explain the codification briefly

explain the objective
Talk about 
