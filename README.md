# rbda_ros2

이 저장소는 RBDA 로봇 관련 ROS2 패키지를 포함하고 있습니다.

## Overview

- **rbda_description**: 로봇의 모델을 정의하는 URDF 및 기타 설명 파일를 담고 있습니다.

## Installation

### Dependencies

- [ROS 2 Humble](https://docs.ros.org/en/humble/Installation.html)

### Build From Source

1. ROS 2 워크스페이스를 생성해주세요.
   ```bash
   mkdir -p ~/rbda_ros2_ws/src
   ```
2. ``rbda_ros2`` 저장소를 클론하고 빌드해주세요.
   ```bash
   cd ~/rbda_ros2_ws
   git clone https://github.com/RainbowRobotics/rbda_ros2.git src/rbda_ros2
   colcon build --symlink-install
   ```

## How to Use

Rviz2 로 RBDA 모델을 시각화합니다.

```bash
source ~/rbda_ros2_ws/install/setup.bash
ros2 launch rbda_description display.launch.py
```