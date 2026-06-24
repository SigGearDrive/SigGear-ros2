# ROS2 Configuration Examples

This folder is reserved for ROS2 configuration examples for SigGear robot joint actuator integration.

Configuration files may include actuator ID settings, CAN bus parameters, joint limits, control mode settings, feedback settings, and safety-related parameters.

## Planned Configuration Topics

This folder may include examples for:

* CAN interface name
* CAN baud rate
* Actuator ID
* Joint name
* Position limits
* Velocity limits
* Torque limits
* Control mode
* Feedback rate
* Fault handling behavior
* Startup behavior
* Emergency stop behavior

## Example Configuration Concept

A typical configuration file may define:

```yaml
siggear_joint:
  joint_name: "joint_1"
  actuator_id: 1
  can_interface: "can0"
  can_baudrate: 1000000
  control_mode: "position"
  position_limit_min: -3.14
  position_limit_max: 3.14
  velocity_limit: 1.0
  torque_limit: 1.0
  feedback_rate_hz: 100
```

The values above are examples only. Final parameters must be confirmed according to the actuator model, firmware version, robot design, and safety requirements.

## Safety Notes

Before using any configuration file:

* Confirm the correct actuator ID.
* Confirm the correct CAN interface.
* Confirm the correct CAN baud rate.
* Set conservative velocity and torque limits for first tests.
* Confirm joint direction and zero position.
* Confirm mechanical limits before motion testing.
* Prepare an emergency stop method.

## Related Documentation

* [ROS2 Robot Joint Actuator](https://siggeardrive.github.io/SigGear-product-docs/Developers/ros2-robot-joint-actuator/)
* [CAN Protocol Robot Joint Control](https://siggeardrive.github.io/SigGear-product-docs/Developers/can-protocol-robot-joint-control/)

## Contact

For confirmed configuration files, ROS2 integration support, CAN protocol details, actuator samples, or custom robotic drive support, contact SigGear:

**Email:** [wangwanrong984@gmail.com](mailto:wangwanrong984@gmail.com)
