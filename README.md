# AI-ROB-Task3

1. installed all these packages:

sudo apt-get update && sudo apt-get install -y \
     ros-humble-joint-state-publisher-gui \
     ros-humble-gazebo-ros \
     ros-humble-xacro \
     ros-humble-ros2-control \
     ros-humble-ros2-controllers \
     ros-humble-joint-state-broadcaster \
     ros-humble-joint-trajectory-controller \
     ros-humble-controller-manager
     ros-humble-moveit \
     ros-humble-gazebo-ros2-control

2. Then follow these comands
   
 - sudo apt install git
 - sudo apt install python3-colcon-common-extensions
 - sudo apt install ros-humble-moveit

4. Add the “Robot_Arm_ROS2” package to “src” folder
   
- source /opt/ros/humble/setup.bash
- mkdir -p ~/ros2_ws/src
- cd ~/ros2_ws/src
- git clone https://github.com/smart-methods/Robot_Arm_ROS2.git
- cd ..
- colcon build
- source ~/ros2_ws/install/setup.bash
 ---
 
## To control the robot arm by joint-state-publisher
- source ~/ros2_ws/install/setup.bash
- ros2 launch arduinobot_description display.launch.py
  
---
<img width="1918" height="1198" alt="Screenshot 2025-11-08 173542" src="https://github.com/user-attachments/assets/6a754312-469d-451f-bd0d-0c72ba30e2e7" />

---

## To control the robot arm by Movit and kinematics
In new terminal:
- source ~/ros2_ws/install/setup.bash
- ros2 launch  arduinobot_mc demo.launch.py

---
<img width="1918" height="1116" alt="Screenshot 2025-11-08 173723" src="https://github.com/user-attachments/assets/bc51f857-d4a1-4b89-8abd-79814b8ba374" />


 
