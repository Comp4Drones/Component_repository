---
title: SCALIAN – EZ_land Precision Landing
componentId: WP4-2
tags: AI, Take-off, Precision Landing, data fusion
---

# EZ_Land Precision Landing

- __ID:__ WP4-2
- __Contributor:__ SCALIAN
- __Owner:__ SCALIAN
- __Licence:__ Proprietary
- __expected TRL:__ 5
- __KET:__ 2.3 Positioning, 2.2.1 Take-off, 2.2.2 Landing, 2.2.7 Obstacle  Detecton and Avoidance, 2.4.1 Data fusion and processing, 3.1.2 Passive Optical
- __Contact:__ david.cherel@scalian.com

The precision landing is a frequent subject for autonomous multicopter because it is an essential component for safety and autonomy in a drone system. Indeed, when relying solely on the GPS signal and IMU data, a drone can have a landing offset up to 5 meters if the signal is bad. Such an offset can be very dangerous: the drone can land on a damaged zone, risking the physical integrity of the drone, or land on a zone with human operators.

To demonstrate the efficiency of such a component, the precision landing will be deployed during the METIS use case (UC3-Demo1) to improve the safety of the system and to facilitate the operations of refill and reload of the drone when landed. It will also be deployed during the use case of ATECHSYS (UC3-Demo2) where the multicopter needs to land precisely on a droid TwinswHeel to pick up and drop off a package. Paired up with the [clearance component](../computer_vision_and_image_processing/SCALIAN-clearance.md) (human detection), the landing will be cancelled if a human is detected near the landing zone, making this component safer.

The goal of the component is to ensure a **safe**, **autonomous** and **precise landing**. 

The component of SCALIAN aims at exploiting the strength of several sensors to ensure a robust, safe and precise landing. To answer the needs of UC3-Demo1 and UC3-Demo2, the sensor IR lock and a computer vision algorithm are integrated in the component.

The visual processing algorithm is specific to a design of helipad (on the right). Aruco type markers are not used to have a more robust algorithm. Shadows and creases have a smaller impact on a refined helipad.

The component is based on a modular architecture that allows the users to configure which sensors are needed. With this conception, it is also easy to integrate a new type of sensor. It is then possible to fine tune the component to the use-case and its constraints.

![Visual processing pipeline](../../img/SCALIAN-ez_land.png)
