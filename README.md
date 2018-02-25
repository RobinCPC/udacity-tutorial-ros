# udacity-tutorial-ros
A simple tutorial of ROS made by Udacity

## How to launch the simulation
Make sure you have all the required ROS packages installed, and that this package is in your ROS workspace (assumed ot be ~/catkin_ws.)

``` bash
cd ~/catkin_ws
# check if need to install required ROS packages
rosdep check --from-paths src --ignore-src --rosdistro=$ROS_DISTRO
# then install with following command or manually use `apt-get install`
rosdep install --from-paths src --ignore-src --rosdistro=kinetic -y
```

If you have not built your workspace do it now (make sure you are inside the workspace root directory):

``` bash
catkin build # or catkin_make
```

Once the simple_arm package has been built, you can launch the simulation environment using:

``` bash
source ~/catkin_ws/devel/setup.bash
roslaunch simple_arm robot_spawn.launch
```

