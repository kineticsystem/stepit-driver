# StepIt Description

This package configures a sample robot that uses the StepIt Driver. The robot is displayed in RViz.

To activate the robot execute the following command:

```
ros2 launch stepit_description robot.launch.py
```

By default, the robot runs on fake hardware. To drive the microcontroller, set the launch arguments `use_dummy`, `usb_port` and `baud_rate`:

```
ros2 launch robot_description robot.launch.py use_dummy:=false usb_port:=/dev/ttyACM0
```

To make the robot move, we need to connect the hardware to a controller. This functionality is implemented in the package `stepit_bringup`.
