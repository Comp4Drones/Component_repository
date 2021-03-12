---
title: IFAT - Component for trusted communication
componentId: WP3-10
tags:
  - security
---

WP3-10

# Component for trusted communication

- __ID:__ WP3-10
- __Contributor:__ IFAT
- __Owner:__ 
- __Licence:__
- __expected TRL:__
- __KET:__
- __Contact:__

IFAT is developing a hardware-security-component (WP5), typically denoted as "Secure Element", and corresponding generic Software-Libraries (WP3). Both parts (HW+SW) combined will be then prepared (as reference-demo) to be integrated by future drone-system-integration partners to raise the overall trustworthiness of their (maybe already existing) communication sub-architecture. Therefore, this component is seen as one important sub-component contributing to an overall _"trusted communication architecture"_.

Shall ensure confidentiality, authenticity and integrity of credentials.

Primary functional focus of this component is:

* the protection of the most critical credentials (e.g. private keys of a PKI) in a temper-resistant storage (to prevent potential extraction if an attacker would obtain physical access to a drone)
* performing essential cryptographic operations during security-critical communication handshake-procedures (e.g. TLS-handshake) in a hardware-secured environment
* to finally achieve secured mutual-authentication of the drone towards various remote stations (e.g. flight control server, or e.g. receiver of camera-date, etc).

---
**Remark**

The purpose of this security-component should not be confused with the authentication of the drone towards the mobile network operator (MNO) for network access. That is usually already done today using standard SIM/eSIM hardware (which is not the purpose of the component developed by IFAT in the course this project).

---
