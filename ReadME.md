# wheel robot
robot having 2 caster wheels and 2 sensors (camera and laser). we have used python (rospy) instead of c++.

# launch

first clone the repo
'''git clone https://github.com/selambeyu/Robotics_Project.git'''
then clone the plugin we made to drive the robot around using keyboard.
'''
    git clone https://github.com/selambeyu/pluginfor_robot.git
'''
* inside catkin_ws/:
```sh
$ chmod u+x src/teleop_twist_keyboard/teleop_twist_keyboard

$ catkin_make

$ source devel/setup.bash
```

launch the robot into gazebo sim

''' roslaunch Robotic_Project spawn.launch '''

then run the plugin
''' rosrun teleop_twist_keyboard teleop_twist_keyboard '''

now you can control the robot with keyboard
start by pressing i
