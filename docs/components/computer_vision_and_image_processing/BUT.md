---
title: BUT algorithms
componentId: WP3-03
tags:
  - architecture
  - hardware
  - SoC
  - video processing
---

# Sensor information algorithms

- __ID:__ WP3-03
- __Contributor:__ BUT
- __Owner:__ 
- __Licence:__
- __expected TRL:__
- __KET:__
- __Contact:__

In this component BUT will implement/improve sensor data processing algorithms  which will include software and firmware for FPGA. This will involve video processing algorithms (for example HDR algorithms). HDR multi-exposure fusion algorithm to be implemented in the drone, possibly implementing also tone mapping and/or ghost removal (with most probably somewhat liited capabilities) in order to "feed" further image and video processing subsystems in the drone by image information with high dynamic range. As a "demonstrator", we can also provide e.g. object detection in HDR.

Increased performance of the algoritms, which will reduce latency and increase throughput.
Robustness of the controller with respect to environmental disturbances and increased resiliency. This improvement will be based on increased robustness of the video processing with respect to HDR while keeping the processing means and extent of video processing "unchanged" thanks to the tone mapping that virtually brings the "same image format" as in usual processing.
