## Setup

```shell
rosdep install -i --from-path src --rosdistro jazzy -y
colcon build
source install/setup.bash
```

## Running

```shell
ros2 launch urdf_tutorial display.launch.py model:=urdf/01-myfirst.urdf
ros2 launch urdf_tutorial display.launch.py model:=urdf/02-multipleshapes.urdf
# etc...
```

## Running r2d2 moving

```shell
colcon build --symlink-install --packages-select urdf_tutorial_r2d2
ros2 launch urdf_tutorial_r2d2 demo.launch.py
rviz2 -d install/urdf_tutorial_r2d2/share/urdf_tutorial_r2d2/r2d2.rviz
```