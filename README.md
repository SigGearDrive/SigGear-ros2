# SigGear ROS2

ROS2 integration package for SigGear robotic joint modules.

## Status

Initial ROS2 integration is based on the `odrive_can` package.

Tested environment:

| Item | Version |
|---|---|
| OS | Ubuntu 23.04 |
| ROS2 | Iron |
| Platform | Linux |

Mac and Windows are not currently supported.

## Supported Products

- SG6010C
- SG8021
- CPM80-25
- CPM100-25

## Installation

Create a ROS2 workspace:

```bash
mkdir -p ~/siggear_ros2_ws/src
cd ~/siggear_ros2_ws/src
git clone https://github.com/odriverobotics/odrive_can
cd ~/siggear_ros2_ws
colcon build --packages-select odrive_can
source ./install/setup.bash
ros2 launch odrive_can example_launch.yaml
ros2 topic echo /odrive_axis0/controller_status
ros2 topic echo /odrive_axis0/odrive_status
ros2 service call /odrive_axis0/request_axis_state /odrive_can/srv/AxisState "{axis_requested_state: 4}"
ros2 service call /odrive_axis0/request_axis_state /odrive_can/srv/AxisState "{axis_requested_state: 8}"
ros2 service call /odrive_axis0/request_axis_state /odrive_can/srv/AxisState "{axis_requested_state: 1}"

Roadmap
Native SigGear ROS2 driver
JointState publisher
URDF models
Gazebo simulation
MoveIt integration
ros2_control hardware interface

---

# 3. 仓库：SigGear-product-docs

## 文件：`SG6010C.md`

直接复制：

```markdown
# SG6010C Robotic Joint Module

SG6010C is a compact planetary robotic joint module for humanoid robots, exoskeletons, quadruped robots and lightweight robotic arms.

## Key Specifications

| Parameter | Value |
|---|---|
| Rated speed | 170 rpm ±10% |
| Maximum speed | 490 rpm ±10% |
| Rated torque | 6.5 Nm |
| Peak / blocking torque | 18 Nm |
| Rated current | 16.5 A |
| Peak current | 50 A |
| No-load current | 0.05 A |
| Phase resistance | 0.158 Ω |
| Phase inductance | 107 μH |
| RPM constant | 104 rpm/V |
| Torque constant | 0.042 Nm/A |
| Weight | 382 g ±3 g |
| Pole pairs | 10 pairs |
| Phase | 3-phase |
| Driver type | FOC |
| Reduction ratio | 9.67:1 |

## Drive Specifications

| Parameter | Value |
|---|---|
| Rated voltage | 15–48 V DC |
| Minimum / Maximum voltage | 12 / 72 V DC |
| Rated current | 6 A |
| Maximum line current | 30 A |
| Maximum phase current | 90 A |
| Standby power consumption | <10 mA |
| Maximum CAN baud rate | 1 Mbps |
| USB Type-C rate | 10 Mbps |
| Encoder resolution | 16-bit absolute single-turn |
| Operating temperature | -20°C to 70°C |
| Motor temperature alarm | 90°C adjustable |
| Drive board temperature alarm | 90°C adjustable |

## Interfaces

- Power and CAN integrated terminal
- USB Type-C debugging interface
- Second encoder interface
- Expansion slot
- SWD debug interface
- Motor temperature interface
- Brake / brake resistor interface
- Limit switch interface

## Applications

- Humanoid robot joints
- Quadruped robot joints
- Exoskeleton joints
- Lightweight robotic arms
- Education and research robots
