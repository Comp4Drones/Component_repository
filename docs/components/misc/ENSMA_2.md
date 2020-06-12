---
title: ENSMA - Multi-agent swarm control
tags:
  - swarm
KET: 
  - Command and Control
  - Obstacle Detection and Avoidance
  - Swarm Formation and Cooperation
---

# Multi-agent swarm control

- __ID:__ WP3-14_2
- __Contributor:__ ENSMA
- __Owner:__ ENSMA
- __Licence:__ LGPL
- __expected TRL:__ 3
- __KET:__ 1.1.6 - Command and Control, 2.2.7 - Obstacle Detection and Avoidance, 2.5.2 - Swarm Formation and Cooperation
- __Contact:__ _patrick.coirault@univ-poitiers.fr_


## Requirements

__UC3-OPR-005__: The GCS shall be able to handle multiple agents or system of agents.

__UC3-OPR-006__: The GCS shall be able to handle different types of agents at the same time.

__UC3-INT-012__: The GCS shall be able to send commands to agents or system of agents.

__UC3-FNC-025__: The GCS shall detect trajectory conflicts between different agents


## Specification

In many practical scenarios, it is required that the agents of Multi-Agent System (MAS) create and maintain a desired geometric shape. The required shape could either be fixed or time-varying. In some cases, it is further required that the agents follow a trajectory while maintaining the shape. The trajectory is produced by a virtual or real leader. This is known as formation tracking.

## Improvements

The aim of this task is to develop distributed consensus and formation of a swarm of drones. From the state of art, it is clear that the available cooperative control schemes do not take various limitations in to account. Motivated by this, the current task focused on the design and implementation of distributed cooperative control laws for a swarm of drones with communication and sensor constraints. These considered constraints are given below:

-	Each drone can only measure its position state
-	Drones are not equipped with sensors to measure their velocity
-	Drones do not have access to the input (control) of their neighbors
-	The measured state is transmitted to the neighbors at irregular and non-uniform time intervals
-	The transmission among the drones is asynchronous and totally independent of other drones in the network
-	The communication topology among the drones may be directed or undirected 
-	The connectivity of the communication network is maintained
-	Both time-varying and fixed formation shape cases are investigated
-	Since inter-agent collision is another important issue in formation tracking control, a potential function based collision avoidance algorithm is incorporated with the proposed formation tracking controller. The collision avoidance algorithm ensures that the drones converge to produce the desired geometric shape without colliding with each other

## Interface

Inputs: 
-	From communication module, Cartesian coordinates of the neighbors 
-	From internal sensor of the drone, Cartesian coordinates and Euler angles
-	Distance to the obstacle from sensor proximity detection

Outputs:
-	Four rotor speed

