## Humanoid Robot Initial Visualisation

This is just to see if our robot design is accurate and will actually stand, and also to implement PID.

Current progress:

|  rviz  |  gazebo  |
| :---: | :---: |
| ![humanoid1](https://github.com/Iqmaa/humanoid_visualisation/blob/main/Media/rviz.png?raw=true)  | ![humanoid2](https://github.com/Iqmaa/humanoid_visualisation/blob/main/Media/gazebo.png?raw=true) |

Training on how to walk and perform other tasks will be done in mujoco.

### Steps to Launch

1. clone the repo
```
git clone (insert link)
```
go into the folder
```
cd humanoid_visualisation
```

2. build the workspace
```
colcon build --symlink-install
```
3. source the workspace
```
source install/setup.bash
```
4. launch the project

#### RViZ alone
```
ros2 launch urdf_tutorial display.launch.py model:=$(pwd)/src/humanoid_description/urdf/humanoid.xacro
```

#### Gazebo

```
ros2 launch humanoid_description gazebo.launch.py
```
