# Ros_6072_basic
Mini Project for Fra502
## Prerequistes
- Ubuntu 18.04
- Ros Melodic 
- Gazebo 9
### Run gazebo and teleop keyboard
Use gazebo and keyboard for simulation
```sh
roslaunch robotblack_gazebo robotblack_gazebo.launch 
```
Use the keyboard only
```sh
roslaunch robotblack_gazebo teleop_Rb.launch 
```
### Navigation and create map
To create map by slam gmapping
```sh
roslaunch robotblack_slam slam_gmapping.launch 
```
Save map with map saving
```sh
rosrun map_server map_saver -f mymap
```
Navigation robot
```sh
roslaunch robotblack_navigation robotblack_navigation.launch
```
