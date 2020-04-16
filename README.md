# BAXTER - Pick and Place in Gazebo
## Installation - Baxter Packages
```
mkdir -p ros_ws/src
cd ~/ros_ws
catkin_make
```

Open - https://sdk.rethinkrobotics.com/wiki/Simulator_Installation and follow the instructions for Baxter and Moveit setup.Make sure to change your ROS distro in baxter.sh file.

## Moveit - Installation and setup
```
sudo apt-get install ros-kinetic-moveit
```
To install other packages for move-it Rviz interface :
```
cd ~/ros_ws/src
git clone https://github.com/ros-planning/moveit_robots.git
cd ..
catkin_make 
```

## Launching an example Baxter Simulation
```
cd ~/ros_ws
./baxter.sh sim
roslaunch baxter_gazebo baxter_world.launch
```

## To run the 2 cube pick and place simulation

```
cd ros_ws/src
git clone https://github.com/SaumilShah66/project4
cd ..
catkin_make
source devel/setup.bash
roslaunch project4 baxter_pick_and_place_demo.launch
```

