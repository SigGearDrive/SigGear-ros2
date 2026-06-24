# ROS2 Launch Examples

This folder is reserved for ROS2 launch file examples for SigGear robot joint actuator integration.

Launch files may be used to start actuator communication nodes, CAN interface nodes, joint command nodes, feedback monitoring nodes, and safety-related monitoring processes.

## Planned Launch File Topics

This folder may include examples for:

* Single robot joint actuator startup
* Multi-actuator CAN bus startup
* Humanoid robot joint actuator launch
* Quadruped robot leg actuator launch
* Robot arm joint actuator launch
* Joint feedback monitoring launch
* Fault status monitoring launch
* Configuration-based actuator startup
* Test mode startup for development and debugging

## Typical Launch Structure

A typical ROS2 launch file may start:

* CAN communication node
* SigGear actuator driver node
* Joint command interface
* Joint feedback publisher
* Fault status monitor
* Optional visualization or logging node

## Example Launch Concept

A typical launch command may look like:

```bash
ros2 launch siggear_ros2 siggear_joint.launch.py
```

A launch file may load parameters from:

```text
config/siggear_joint.yaml
```

The exact package name, launch file name, node name, topic name, and parameter file may vary depending on the final ROS2 package structure.

## Safety Notes

Before running any launch file:

* Confirm the actuator is mechanically secured.
* Confirm the correct CAN interface.
* Confirm the correct CAN baud rate.
* Confirm actuator ID settings.
* Use conservative velocity and torque limits.
* Test one actuator before testing multiple actuators.
* Monitor fault feedback continuously.
* Prepare an emergency stop method.

## Related Documentation

* [ROS2 Robot Joint Actuator](https://siggeardrive.github.io/SigGear-product-docs/Developers/ros2-robot-joint-actuator/)
* [CAN Protocol Robot Joint Control](https://siggeardrive.github.io/SigGear-product-docs/Developers/can-protocol-robot-joint-control/)
* [SigGear Robot Joint SDK](https://github.com/SigGearDrive/SigGear-robot-joint-sdk)

## Contact

For confirmed ROS2 launch files, actuator configuration support, CAN protocol details, samples, or custom robotic drive integration support, contact SigGear:

**Email:** [wangwanrong984@gmail.com](mailto:wangwanrong984@gmail.com)
