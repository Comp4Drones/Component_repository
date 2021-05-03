---
title: IKERLAN - Safety function - Pre-Certified SOM
componentId: WP3-01
tags:
  - Detect and Avoid
  - LIDAR
---

WP3-01

# Safety function - Pre-Certified SOM

- __ID:__ WP3-01
- __Contributor:__ IKERLAN
- __Owner:__
- __Licence:__ Proprietary
- __expected TRL:__
- __KET:__
- __Contact:__

The Ikerlan Mammut computer module enables the use of heterogeneous computing capabilities in drone
systems. These systems traditionally have a limited computing power to execute complex algorithms,
such as obstacle detection and avoidance, object recognition or neural network execution, and process
data from sensors such as cameras or LiDARs.  The Mammut computer module enables the integration of
those functionalities.

Mammut has been designed with modularity and reusability in mind. For such purposes, it complies with the
[SMARC standard](https://sget.org/), a SGET association standard which establishes the size, exposed
interfaces, electric characteristics and pin-out for embedded computer modules. This allows the reuse of
computer modules in different use-cases, exchanging the carrier board where is plugged. Thanks to this,
the user can cut the development time, allowing a shorter time to market and overall development
cost of new products and solutions.

In the project scope, provides hardware blueprint for testing and integrating the modular approach of the reference architecture,
that is composed of different building blocks. The carrier board that has been designed enables the connection of widely-used sensors
and the communication with various autopilots.

The integration in drone architecture is done using Flight Controller Unit - Companion Computer architecture. This is the default architecture
in drone systems to aggregate additional computing capabilities to a commercial drone. For instance, it is used in DJI products, PX4-based or ArduPilot based drones.

![](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdiscuss.ardupilot.org%2Fuploads%2Fdefault%2Foriginal%2F2X%2Fd%2Fda4a5fa812b41784bc33335e041d3f0aeaf4788f.jpg&f=1&nofb=1 "RPi to Pixhawk FCU")
