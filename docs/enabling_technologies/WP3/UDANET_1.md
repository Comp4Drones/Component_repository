---
title: UDANET - Smart and predictive energy management system
componentId: WP3-36_1
---


# WP3-36_1 - Smart and predictive energy management system

|||
|-|-|
|ID|WP3-36_1|
|Contributor|UDANET|
|Levels|Functional|
|Require|Sensors that provide measurements and mission details|
|Provide|Energy trajectories to perform path tracking missions|
|Input|X, Y, Z coordinates of the drone and its velocities<br/>Roll, pitch, and yaw angles of the drone<br/>Initial and final position of the mission|
|Output|Rotor’s speed (or forces) |
|C4D building block|Flight planning|
|TRL|3-4|

## Detailed Description

An energy management system is vital to optimize the energy life and the purpose of the system. It will continuously monitor important system parameters, while dealing with the varying power demands of the many aspects, the objectives of the mission and optimizing the usage of the energy. Given the initial and final positions, the objective of the component is to compute the control inputs that rule the motion and vehicle trajectory to optimize energy consumption and the computational burden of the algorithm.

The aim of this activity is to use a model-based approach to control UAV flight to minimize energy consumption. It is therefore necessary to consider the flight dynamics, battery, and energy flow and actuator models. The strategy that led to good results in some research is the optimal control and therefore this type is considered in the activity. A first objective is to improve control by making it robust with respect to model approximation errors or disturbance (for example under wind conditions). 

## Contribution and Improvements

The main contribution of the component is to provide excellent trajectories from an energy point of view for the position, speeds that are the result of an elaboration of the associated optimal control problem and analysis of the excellent results. The improvement is due to the fact that a real-time resolution of the control is not required, but rule-based strategies are required which therefore have a low computational cost. Furthermore, in collaboration with other partners, they want to experiment in non-ideal conditions (presence of wind)

## Design and Implementation

The designed energy management system will be verified and tested via Software in The Loop using software Matlab-Simulink. The reference generator will be implemented to execute a mission and the associated controller and will be tested both with Matlab-Simulink and with complex simulators in less than ideal conditions.


