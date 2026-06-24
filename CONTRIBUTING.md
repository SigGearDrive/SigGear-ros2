# Contributing to SigGear ROS2 Resources

Thank you for your interest in SigGear ROS2 integration resources.

This repository provides reference materials, examples, and documentation for integrating SigGear robot joint actuators, compact cycloidal robotic joint modules, CAN-based actuator control, and robotic drive systems with ROS2.

## Contribution Scope

Contributions may include:

* ROS2 node examples for robot joint actuator control
* ROS2 launch file examples
* Configuration file examples
* CAN bus integration notes
* Joint command and feedback examples
* Documentation improvements
* Testing utilities
* Safety and fault handling references
* Integration notes for humanoid robots, quadruped robots, robot arms, and robotic grippers

## Before Contributing

Before submitting a contribution, please make sure that:

* The contribution is relevant to SigGear robot joint actuator integration.
* Example code is clearly documented.
* Topic names, message structures, CAN IDs, and control parameters are marked as examples unless confirmed by SigGear.
* Safety-related behavior is described carefully.
* Product-specific values are not presented as universal values.

## Safety Notice

Robot joint actuators and motor control systems can generate high torque, high speed, and unexpected motion.

Before testing any ROS2 actuator example:

* Secure the actuator mechanically.
* Confirm wiring, voltage, CAN baud rate, and actuator ID.
* Use low speed and low torque limits for first tests.
* Keep clear of moving parts.
* Prepare an emergency stop method.
* Monitor fault feedback continuously.
* Do not run motion tests on an unsecured actuator.

## Documentation Style

Please use clear technical English.

When adding ROS2 examples, include:

* Required hardware
* Required software
* ROS2 version
* CAN interface assumptions
* Topic names
* Message format
* Launch command
* Configuration file example
* Safety notes
* Expected behavior
* Known limitations

## Contact

For ROS2 integration support, CAN protocol details, actuator samples, CAD files, datasheets, or custom robotic joint drive support, contact SigGear:

**Email:** [wangwanrong984@gmail.com](mailto:wangwanrong984@gmail.com)
