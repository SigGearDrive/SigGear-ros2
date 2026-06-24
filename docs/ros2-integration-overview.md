# ROS2 Integration Overview for SigGear Robot Joint Actuators

This page provides a general ROS2 integration overview for SigGear robot joint actuators, compact cycloidal robotic joint modules, and CAN-based robotic drive systems.

The information here is intended for engineering reference only. Final topic names, message definitions, CAN IDs, control modes, feedback data, fault codes, and safety logic may vary by product model, firmware version, motor configuration, and customer-specific requirements.

## Typical ROS2 Architecture

A typical SigGear ROS2 actuator integration may include:

* ROS2 control computer
* CAN interface adapter
* CAN communication layer
* SigGear robot joint actuator
* Joint command node
* Joint feedback node
* Fault monitoring node
* Launch file
* Configuration file
* Safety handling logic

## Example ROS2 Topic Structure

Example topic names may include:

```text
/siggear/joint_command
/siggear/joint_feedback
/siggear/joint_status
/siggear/fault_state
```

These topic names are examples only. Final topic names may be adjusted based on project architecture.

## Typical Command Data

A robot joint command message may include:

* Joint ID
* Control mode
* Target position
* Target velocity
* Target torque
* Enable or disable command
* Motion limit parameters

## Typical Feedback Data

A robot joint feedback message may include:

* Joint ID
* Actual position
* Actual velocity
* Estimated torque
* Motor current
* Bus voltage
* Temperature
* Actuator state
* Fault code

## Common ROS2 Use Cases

SigGear ROS2 resources can support integration for:

* Humanoid robot knees, hips, ankles, shoulders, and elbows
* Quadruped robot hip and knee actuators
* Robot arm shoulder, elbow, and wrist joints
* Robotic grippers and compact end effectors
* CAN-based multi-actuator robotic systems
* Research robot platforms
* Compact automation systems

## Safety Considerations

Before running ROS2 actuator tests:

* Confirm actuator wiring and power supply.
* Confirm CAN baud rate and actuator ID.
* Start with low speed and low torque limits.
* Test one actuator before multi-actuator operation.
* Monitor feedback and fault state continuously.
* Prepare an emergency stop method.
* Avoid running motion tests on unsecured actuators.

## Related Documentation

* [ROS2 Robot Joint Actuator](https://siggeardrive.github.io/SigGear-product-docs/Developers/ros2-robot-joint-actuator/)
* [CAN Protocol Robot Joint Control](https://siggeardrive.github.io/SigGear-product-docs/Developers/can-protocol-robot-joint-control/)
* [Robot Joint Gearbox Selection Guide](https://siggeardrive.github.io/SigGear-product-docs/Selection-Guides/robot-joint-gearbox-selection-guide/)

## Contact

For confirmed ROS2 examples, CAN protocol documents, actuator samples, or custom integration support, contact SigGear:

**Email:** [wangwanrong984@gmail.com](mailto:wangwanrong984@gmail.com)
