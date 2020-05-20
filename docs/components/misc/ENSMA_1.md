---
title: ENSMA - Control components that implement potential barriers
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

## Improvements

