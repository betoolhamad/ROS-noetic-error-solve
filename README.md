# ROS-noetic-error-solve
The soulation of ROS noetic, which has an error when trying to run the robot arm package in Rviz. 

To run robot arm pakage using command :

```
$ roslaunch robot_arm_pkg check_motors.launch
```

It's will shown this error :

```
ERROR: cannot launch node of type [robot_state_publisher/state_publisher]: Cannot locate node of type [state_publisher] in package [robot_state_publisher]. 
Make sure file exists in package path and permission is set to executable (chmod +x)
```

**The soulation is simple, we need to change the type of file that we want to run it in RViz, which is called check_motors.launch.**

We will change the type from type='joint_state_publisher' to type='robot_state_publisher'

<img width="600" alt="Solve" src="https://user-images.githubusercontent.com/43522153/122856397-65c83a80-d31f-11eb-96e7-a063e5d41545.png">







