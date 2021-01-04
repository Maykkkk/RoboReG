---
title: Underactuated Attitude Control of Small Satellites

description: |
  Developing algorithms and hardware for underactuated control of small satellites, mainly through trajectory optimization techniques of magnetorquer attitude manipulation.

people:
  - zac
  - andrew

layout: project
image: "/img/underactuated_cubesat.gif"
last-updated: 2019-09-27
---

Due to the ever-increasing scope of small satellite missions, there is now significant demand for precise attitude determination and control capabilities onboard CubeSats. Interactions between magnetic torque coils and the Earth’s magnetic field have been used for decades onboard satellites to offload momentum from reaction wheels and control-moment gyroscopes. However, magnetorquers are inherently underactuated, and mechanical actuators like reaction wheels are often prohibitively expensive in terms of mass, volume, power, and cost for CubeSat missions.

This research investigates magnetorquer-only attitude control technique that utilizes trajectory optimization to circumvent the under-actuated nature of satellite magnetic field interactions. Given a known orbit and desired attitude state, current methods utilize a simplified dynamics model and a fast constrained trajectory optimization solver based on differential dynamic programming to arrive at a nominal torque profile that respects the spacecraft’s actuator limitations and desired actuation efficiency. Nominal maneuvers are then tracked online using a time-varying linear-quadratic regulator (LQR).

Future work includes implementation of the algorithm to embedded hardware through a flat-sat prototype. This will involve base-level programing and component selection. Once the system has been validated, the attitude dynamcis will be fed into the hardware and the system's resulting control inputs can then be compared to simulation.  
