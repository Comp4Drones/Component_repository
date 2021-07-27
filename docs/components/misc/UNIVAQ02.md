---
title: UNIVAQ - Autonomy, cooperation, and awareness
componentId: WP4-33
tags:
  - Control
---

# Autonomy, cooperation, and awareness

- __ID:__ WP4-33
- __Contributor:__ UNIVAQ
- __Owner:__ UNIVAQ
- __Licence:__ OPEN SOURCE
- __expected TRL:__ 3-4
- __KET:__ Command and control; Intelligent Mission Management; Obstacle Detection and Avoidance.
- __Contact:__ Stefano Di Gennaro (stefano.digennaro@univaq.it); Mario Di Ferdinando (mario.diferdinando@univaq.it).

Autonomy, cooperation, and awareness.

The provided component concerns a robust digital algorithm for the autonomous navigation and cooperation of UAVs. In particular, the proposed digital control system is designed by 
taking simultaneously into account: the presence of sampling and quantization in the used devices; the presence of external disturbances such as measurement uncertainties and 
environment perturbations. The proposed control algorithm is able to arbitrarily attenuate the effects of such external disturbances and allows the main swarm cooperative 
strategies, namely time-varying flight formation, swarm tracking, and social foraging. The proposed control strategy includes also functionalities for the obstacle avoidance and 
the collision avoidance between adjacent members of the swarm. Limitations in the communication network are also considered. Indeed, the case in which each UAV can communicate with
only a subset of the swarm is included. The external disturbances are unknown for the proposed control algorithm and no estimators are designed for the involved disturbances. The 
only knowledge required by the controller for attenuating external disturbances is their bound. An efficient strategy for the implementation on FPGAs of the proposed control 
algorithm is also presented. In particular, the proposed methodology is mainly focused on retiming and pipelining which allows: (i) lower execution times, and hence smaller 
sampling times, than its naive implementation; (ii) to take into account the energetic aspects of the controller implementations, and not only the controller performance. The 
proposed control strategy relies on methodology recently introduced in [1]-[7].

The proposed control algorithms have been tested through simulations. An analysis of the efficacy of the proposed digital controller was performed by considering very hard actuation 
disturbances affecting the propellers. The simulations show that the proposed robust digital controller achieves very good performances with respect to the same control strategy 
devoid of the new robust control term. In Fig. 1, the desired trajectory of the UAV is plotted with yellow line and the trajectory of the UAV, in the case of robustified and 
non-robustified controller is shown with blue and red line, respectively. 

![plot_xyz_ref_trajectory_1](https://user-images.githubusercontent.com/83577527/127151048-872c3309-1521-4bf7-8672-015c14fa98a7.jpg)

In Fig. 2, the trajectory of the swarm of UAVs, in the case of robustified and non-robustified controller, is shown with black and red line, respectively.

![trajectory](https://user-images.githubusercontent.com/83577527/127151220-85e3172b-92a7-4662-ae86-5389a35dd3a7.jpg)

In the proposed figures, the efficacy of the robust controller with respect to the non-robustified one is evident.
