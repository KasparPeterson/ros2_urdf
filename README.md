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