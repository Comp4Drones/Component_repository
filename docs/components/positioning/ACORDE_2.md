---
title: ACORDE - Multi-antenna GNSS/INS based navigation
componentId: WP3-15_2, WP4-16, WP5-11
tags:
  - hardware
  - positioning
  - data fusion
  - outdoor
---

# Multi-antenna GNSS/INS based navigation

- __ID:__ WP3-15_2, WP4-16, WP5-11
- __Contributor:__ ACORDE
- __Owner:__ ACORDE
- __Licence:__ Private
- __expected TRL:__ 5
- __KET:__ (Outdoor) Positioning
- __Contact:__ fernando.herrera@acorde.com

In COMP4DRONES, ACORDE develops GLAD+, an improved version of its multi-GNSS Low-cost position and Attitude Determination (GLAD) systems (see [ACORDE products](https://www.acorde.com/products) and [GLAD project site](https://glad2-project.acorde.com/)).

![ACORDE_GLAD_plus_flying](../../img/ACORDE_GLAD_plus_flying.jpg "GLAD+ Dragonfly (4 GNSS receivers version) flying on a drone of FADA-CATEC")
*(photo courtesy of FADA-CATEC)*

__Solution:__

GLAD+ provides a trustable, geo-referenced position and attitude based on the fusion of multi-antenna/multi-receiver data and of additional sensors like accelerometers, gyroscopes and barometer.
For it, advanced data fusion and navigation algorithms are employed, adapting and exploiting each navigation profile (drone, land-vehicle, etc). 
Work in C4D focuses on drone profile, a bit more challenging as it prevents some aidings and assumptions usable on other profiles.

<!-- Maybe add FIGURE SCHEME SW -->


__Improvements:__ 

GLAD+ provides a bunch of improvements with regard to GLAD.
HW platform is improved while keeping its reduced cost.
GLAD+ HW integrates multi-constellation receivers, with and anti-jamming and anti-spoofing capabilities, to provide GLAD+ a qualitative performance upgrade in terms of robustness and integrity.

![ACORDE_GLAD_board](../../img/ACORDE_GLAD_board_white_bck.jpg "Zenithal view of GLAD+ Dragonfly (4 GNSS receivers version)")

At software level, GLAD+ platform support a main upgrades (new RTOS port, drivers adaptation and enhancements) to keep a highly competitive solution in terms of cost.

Moreover, GLAD firmware is being upgraded in several aspects of its internal algorithms for a more robust and accurate attitude estimation.

__Interfaces:__ 

TBC (images of HW interfaces, SDK, Mavlink)
