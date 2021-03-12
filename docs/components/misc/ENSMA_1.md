---
title: ENSMA - Control components that implement potential barriers
componentId: WP3-14_1
tags:
  - geofencing
  - navigation
KET:
  - Geofencing
  - Command and Control
  - Detect and Avoid
  - Obstacle Detection and Avoidance
  - Geofencing
---

# Control components that implement potential barriers

- __ID:__ WP3-14_1
- __Contributor:__ ENSMA
- __Owner:__ ENSMA
- __Licence:__ LGPL
- __expected TRL:__ 4
- __KET:__ 1.1.2 - Geofencing, 1.1.6 - Command and Control, 1.3.3 - Detect and Avoid, 2.2.7 - Obstacle Detection and Avoidance, 2.3.2 - Geofencing
- __Contact:__ _patrick.coirault@univ-poitiers.fr_


## Requirements

__UC3-FNC-002__: The dropping agents shall ensure, with a dedicated software, the clearance of a drop location before dropping a sensor.

__UC3-PRF-002__: The clearance algorithm shall run on an embedded computer inside the UAVs. It shall not impact the capability of the UAVs to operate their mission.

__UC3-FNC-05__: SYSTEM shall include an autonomous detect & avoid capability

__UC3-DEM6-FNC-02__: SYSTEM shall include an autonomous detect & avoid capability


## Specification

A control loop that implements a "potential field" that prevents the drone to access certain areas by evaluating its position, geofences and potential obstacles in the environment.

It is assumed that drone is equipped with proximity sensors and can detect any relative position of both non-cooperative and cooperative entities within a sensing range. A cooperative entity is another drone which have the same capability. In contrary, a non-cooperative entity is an entity without collision avoidance system. 

Sensing capability is required to sense the presence of any other entities in its close vicinity which may lead to a collision. These sensors only give the relative position of any entity in its range in the local frame and do not provide position information in the global frame. It is to note that this assumption is used for the purpose of collision avoidance only.

## Improvements

The autonomous flight control includes a mechanism to avoid collision between the drones, obstacles and/or virtual barriers. 

An Artificial Potential Field (APF) method is used for collision avoidance. In APF, a drone is considered as a point in a potential field. This drone experiences a repulsion force from the obstacles and therefore, instead of colliding with them, it steers around them. 

Typically, potential functions are based on the relative distance between drone and the obstacle and do not require any global information. 
Based on the practical aspects, an ideal potential function must have the following properties:

- The range of the potential field must be bounded. Usually, it depends on the range of obstacle sensors mounted on the agent
- The value of the potential field and the corresponding repulsion must be infinity at the boundary of the obstacle and must decrease with the increase in the distance
- First and second derivatives of the potential function must exist in order to have a smooth repulsion force

APF based repulsion mechanism is combined with the control algorithm.

## Interface

Inputs: 
-	Distance to the obstacle from sensor proximity detection
-	Cartesian coordinates and Euler angles of the drone

Outputs:
-	Four rotor speed

