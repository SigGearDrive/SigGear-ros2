# SigGear ROS2 Resources

ROS2 integration resources for SigGear robot joint actuators, compact cycloidal robotic joint modules, CAN-based actuator control, and robotic drive system development.

This repository is intended for robotics engineers, ROS2 developers, embedded engineers, and research teams working on humanoid robots, quadruped robots, robot arms, robotic grippers, mobile robots, and compact automation systems.

## Official Product Documentation

* [SigGear Product Docs](https://siggeardrive.github.io/SigGear-product-docs/)
* [ROS2 Robot Joint Actuator](https://siggeardrive.github.io/SigGear-product-docs/Developers/ros2-robot-joint-actuator/)
* [CAN Protocol Robot Joint Control](https://siggeardrive.github.io/SigGear-product-docs/Developers/can-protocol-robot-joint-control/)

## Related Robot Joint Products

* [CPM100-25 Compact Cycloidal Robotic Joint Module](https://siggeardrive.github.io/SigGear-product-docs/CPM100-25/)
* [CPM80-25 Compact Cycloidal Robotic Joint Module](https://siggeardrive.github.io/SigGear-product-docs/CPM80-25/)
* [SG6010C Compact Precision Drive Solution](https://siggeardrive.github.io/SigGear-product-docs/SG6010C/)
* [SG8021 Precision Drive Solution](https://siggeardrive.github.io/SigGear-product-docs/SG8021/)

## ROS2 Integration Focus

This repository may include ROS2 reference resources for:

* Robot joint actuator control
* CAN-based actuator communication
* Joint command and feedback topics
* Position, velocity, and torque control references
* Actuator state monitoring
* Fault reporting and safety status handling
* Humanoid robot joint integration
* Quadruped robot leg joint integration
* Robot arm actuator integration
* Robotic gripper actuator integration

## Typical ROS2 Use Cases

SigGear ROS2 resources can support development for:

* Humanoid robot knees, hips, ankles, shoulders, and elbows
* Quadruped robot hip and knee actuators
* Robot arm shoulder, elbow, and wrist joints
* Robotic grippers and compact end effectors
* Research robot platforms
* CAN-based multi-actuator robotic systems
* Compact automation systems using ROS2 control architecture

## Related Application Pages

* [Cycloidal Reducer for Humanoid Robot Joints](https://siggeardrive.github.io/SigGear-product-docs/Applications/humanoid-robot-joint-reducer/)
* [Quadruped Robot Joint Gearbox](https://siggeardrive.github.io/SigGear-product-docs/Applications/quadruped-robot-joint-gearbox/)
* [Robot Arm Joint Gearbox](https://siggeardrive.github.io/SigGear-product-docs/Applications/robot-arm-joint-gearbox/)
* [Robot Gripper Gear Motor](https://siggeardrive.github.io/SigGear-product-docs/Applications/robot-gripper-gear-motor/)

## Selection and Comparison Resources

* [Robot Joint Gearbox Selection Guide](https://siggeardrive.github.io/SigGear-product-docs/Selection-Guides/robot-joint-gearbox-selection-guide/)
* [Cycloidal Reducer vs Harmonic Drive](https://siggeardrive.github.io/SigGear-product-docs/Comparisons/cycloidal-vs-harmonic-drive/)
* [Planetary vs Cycloidal Gearbox](https://siggeardrive.github.io/SigGear-product-docs/Comparisons/planetary-vs-cycloidal-gearbox/)
* [Integrated Robot Joint vs Separate Motor Gearbox](https://siggeardrive.github.io/SigGear-product-docs/Comparisons/integrated-robot-joint-vs-separate-motor-gearbox/)

## SDK and CAD Resources

For actuator SDK references and mechanical integration resources, see:

* [SigGear Robot Joint SDK](https://github.com/SigGearDrive/SigGear-robot-joint-sdk)
* [SigGear CAD Models](https://github.com/SigGearDrive/SigGear-cad-models)

## Example ROS2 Architecture

A typical SigGear ROS2 actuator integration may include:

* ROS2 node for actuator communication
* CAN interface layer
* Joint command topic
* Joint feedback topic
* Fault status topic
* Launch file for actuator startup
* Configuration file for actuator ID, CAN baud rate, joint limits, and control mode

Example topic structure:

```text
/siggear/joint_command
/siggear/joint_feedback
/siggear/joint_status
/siggear/fault_state
```

## Notes

The ROS2 resources in this repository are intended as integration references. Final topic names, message definitions, CAN IDs, control modes, feedback data, fault codes, and safety logic may vary by product model, firmware version, motor configuration, and customer-specific requirements.

Before production integration, please confirm the actuator model, electrical interface, CAN communication parameters, ROS2 control requirements, joint limits, safety logic, and feedback format with SigGear.

## Contact

For ROS2 integration support, CAN protocol details, actuator samples, CAD files, datasheets, or custom robot joint drive solutions, contact SigGear:

**Email:** [wangwanrong984@gmail.com](mailto:wangwanrong984@gmail.com)
