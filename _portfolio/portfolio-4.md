---
title: "Composition and Rendering of Bharatanatyam Performance in Augmented Reality"
collection: projects
permalink: /projects/BharatnatyamAR
excerpt: 'This work is about using Blender&#39;s Python API to create dance animations from a list of vectors'
---

{% include base_path %}

[Github Code Repository link](https://github.com/SiddharthSaravanan/BharatanatyamAR)
<br />
[Project Report](https://www.researchgate.net/publication/351559537_Composition_and_Rendering_of_Bharatanatyam_Performance_in_Augmented_Reality)


The objective of this project was to write a program using [Blender's](https://www.blender.org/) [Python API](https://docs.blender.org/api/current/index.html) That is capable of taking a list of 30-dimensional vectors and creating an animation of a dancer. Or simply put, we want to use this:
```
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
1 -1 2 0 2 -1 3 -1 -1 -1 3 0 1 1 2 1 1 1 0 2 2 0 0 0 -3 1 1 0 0 0
2 1 2 0 2 -1 3 -1 1 1 3 0 1 1 2 1 0 0 0 0 0 1 0 0 0 1 1 0 0 0
2 1 2 0 2 -1 3 -1 1 1 6 4 -2 0 2 0 0 0 0 0 0 1 0 0 0 1 1 0 0 0
2 1 2 1 2 0 3 0 0 0 0 2 -1 1 3 -1 0 0 0 0 0 0 0 0 0 0 1 0 0 0
1 -1 2 -2 2 0 2 0 0 0 0 2 -1 1 3 -1 0 0 0 0 0 0 0 0 0 0 1 0 0 0
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 
```

To create this:

![Alt Text](https://media.giphy.com/media/mPgCNQh8b4qVl6EhKk/giphy.gif?cid=790b7611fc09703cd5ccb5306c7d03e060e8193d101e2c52&rid=giphy.gif&ct=g)


# Codification of a Bharathnatyam pose

The Codification of a pose in Bharathanatyam into a 30-dimensional vector was done by professor Sangeeta Jadhav, Goa University (2018). In her work, positions of different parts of the body are represented by different integers within the 30-dimensional vector as shown below:


>Position of Head : 1 and 2,<br />
>Position of Right Hand : 3 to 10,<br />
>Position of Left Hand : 11 to 18,<br />
>Waist position : 19 and 20,<br />
>Right Leg position : 21 to 25,<br />
>Left Leg position : 26 to 30.<br />

Therefore, from a list of 30-dimensional vectors, we can get a list of poses that we can use as keyframes in creating the animation of the dancer.

# Object Oriented design to manipulate the dancer

Once we had created the 3d model, its armature and completed the rigging, We came up with an object-oriented design to set the pose of the dancer based on the 30-dimensional vector. The design had to be such that the dancer would not be able to assume any pose that is not anatomically possible. The challenge was that the possible configurations a particular bone can take depended on the configuration of its parent bones. For example, the possible configuration of the palm depends on the current configuration of the forearm.<br />
To deal with this we created a design that would alter the poses of the bones from the top to the bottom of the bone hierarchy; Starting from the pelvis bone to the finger and the feet bones. This process is depicted in the below diagram:

![image](../images/Main.png)

The overall design is depicted in this UML diagram (svg):

![image](../images/UML_diag_final.svg)

<br />
For more details refer to the [report](https://www.researchgate.net/publication/351559537_Composition_and_Rendering_of_Bharatanatyam_Performance_in_Augmented_Reality)



