# ROS2 Examples

This folder is reserved for ROS2 example resources for SigGear robot joint actuator integration.

The examples in this folder are intended to help engineers understand basic ROS2 actuator communication flow, CAN-based robot joint control, command publishing, feedback reading, and fault monitoring.

## Planned Example Topics

This folder may include examples for:

* Single joint actuator control
* Position command example
* Velocity command example
* Torque command example
* Joint feedback subscription
* Fault status monitoring
* CAN-based actuator communication
* Multi-actuator control reference
* Humanoid robot joint control reference
* Quadruped robot leg actuator reference
* Robot arm joint actuator reference
* Robotic gripper actuator reference

## Typical ROS2 Development Environment

A typical ROS2 development environment may include:

* Ubuntu Linux
* ROS2
* CAN interface adapter
* CAN bus driver
* SigGear robot joint actuator
* Power supply
* Mechanical test fixture
* Emergency stop method

## Example Topic Concepts

Example ROS2 topics may include:

```text
/siggear/joint_command
/siggear/joint_feedback
/siggear/joint_status
/siggear/fault_state
```

These topic names are examples only. Final topic names may be adjusted according to the robot software architecture.

## Example Workflow

A typical ROS2 actuator test workflow may include:

1. Connect the CAN interface.
2. Confirm the actuator ID and CAN baud rate.
3. Start the actuator communication node.
4. Enable the actuator.
5. Send a low-speed or low-torque test command.
6. Read joint feedback.
7. Monitor fault status.
8. Stop or disable the actuator after testing.

## Safety Notes

Before running any ROS2 example:

* Secure the actuator before motion testing.
* Confirm wiring and power supply.
* Confirm CAN interface and baud rate.
* Start with low speed and low torque limits.
* Keep hands and tools away from moving parts.
* Monitor feedback and fault state continuously.
* Prepare an emergency stop method.

## Related Documentation

* [ROS2 Robot Joint Actuator](https://siggeardrive.github.io/SigGear-product-docs/Developers/ros2-robot-joint-actuator/)
* [CAN Protocol Robot Joint Control](https://siggeardrive.github.io/SigGear-product-docs/Developers/can-protocol-robot-joint-control/)
* [Robot Joint Gearbox Selection Guide](https://siggeardrive.github.io/SigGear-product-docs/Selection-Guides/robot-joint-gearbox-selection-guide/)

## Contact

For confirmed ROS2 example files, CAN protocol details, actuator samples, CAD files, datasheets, or custom robot joint drive support, contact SigGear:

**Email:** [wangwanrong984@gmail.com](mailto:wangwanrong984@gmail.com)
