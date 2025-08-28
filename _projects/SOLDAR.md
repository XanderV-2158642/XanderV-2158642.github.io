---
layout: page
title: "SOLDAR"
description: "Supporting low volume pcb prototyping using collaborative robots"
technologies: ["CPP", "Unity", "Augmented reality development", "6DOF robot programming"]
featured: true
date: 2024-10-08
---

## What is SOLDAR

SOLDAR is the product of my bachelor thesis, initially starting as a system to aid in soldering. Starting simple with the intention of using a cobot to help in the soldering process by moving and rotating the Circuitboard based on the component placement, it has grown to a system aiding in both soldering, and feedforward to the user using augmented reality.

## How does SOLDAR work?
SOLDAR takes in 1 file, exportable out of your PCB editor, called a position file. It contains all components that need to be mounted on the board, their name, position, and rotation.

Using this info we a simulation is done to create groups of components that can be placed on the board, without the legs of the components interfering to reach other components.
The initial order the simulation uses is based on standard soldering conventions, mainly small components first, large ones later. 
In each of these group the components are ordered based on the angle of which the reachability is the highest. This is done so the robot can continuously rotate the board in one direction, resulting in a larger efficiency.

Using this grouped process a user places a group of components on the board, following the instructions received in augmented reality. The cobot then flips over the board so the user can solder the components to the board.
After soldering a component the user needs to do a tapping gesture with the right hand, and the system will rotate the board to facilitate soldering for the next component in that group.

This process is repeated until all components are soldered to the board.

Read the abstract sent in to VRST, or check out the poster for a more visual presentation of the system:
[ACM abstract](https://dl.acm.org/doi/abs/10.1145/3641825.3689496) • [Poster](/assets/pdfs/PosterVRST.pdf)
