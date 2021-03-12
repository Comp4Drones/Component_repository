---
title: UWB - Autonomous drone battery management
componentId: WP3-26
tags:
  - plop
---

WP3-26

# Droneport: an autonomous drone battery management system

- __ID:__ WP3-26
- __Contributor:__ UWB
- __Owner:__ 
- __Licence:__
- __expected TRL:__
- __KET:__
- __Contact:__

Droneport (DP) is a complex system for autonomous drone battery management. It can either change battery packs or fast charge small drones. 

## Droneport HW architecture

Droneport consists of

- Drone landing place with landing markers or beacons
- Battery exchange unit  / robotic manipulator
- Battery management unit for charging and storage
- Wireless communication to the drone/swarms
- Optional wired power connection to the drone on the Droneport

## Droneport SW architecture

Droneport SW architecture consists of

- Drone to DP communication protocol
- Drone landing assistant
- Battery exchange system control
- Charge control
- Battery management software

DP software provides open API for interoperability with various drones flight controllers.

## PX4 and Mavlink extensions for autonomous drone battery management

MAVLink is a very lightweight messaging protocol with hybrid publish-subscribe communication with drones and between onboard drone components. (see https://mavlink.io/en/)
PX4 is a complex flight control software widely used in drone community. It performs various basic flight controls and mission tasks. (see  https://px4.io)
The goal is to create MAVLink extensions via messages specialized for autonomous drone battery management (Drone Port). These extension modules will cover the communication messages prepared for MAVLink library auto generation process. The messages will be subsequently implemented to PX4.
