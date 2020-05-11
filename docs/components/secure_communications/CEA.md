---
title: CEA - TSN Queue Mapper
tags:
  - communication
---

WP3-32_1

# TSN Queue Mapper

On the drone, it is expected that communications between different components could be supported by a TSN Network (Time-Sensitive Network). TSN is a group of IEEE Standards that targets support of deterministic communications over standard Ethernet. Several traffic Queues can be defined to support different levels of TSN support (determinism, controlled latency, best efforts, etc.). This software is in charge of setting up the TSN queues and the routing rules so that Traffic with specific QoS requirements can be handled as expected in the TSN network (on-board).

This software is required to setup the TSN flows.
