# wheel robot
robot having 2 caster wheels and 2 sensors (camera and laser). we have used python (rospy) instead of c++.

# launch

first clone the repo
'''git clone https://github.com/ezedinff/wheel_robot.git'''
then clone the plugin we made to drive the robot around using keyboard.
'''
    git clone https://github.com/ezedinff/teleop_twist_keyboard.git
'''

* inside catkin_ws/:
```sh
$ chmod u+x src/teleop_twist_keyboard/teleop_twist_keyboard

$ catkin_make

$ source devel/setup.bash
```

launch the robot into gazebo sim

''' roslaunch wheel_robot spawn.launch '''

then run the plugin
''' rosrun teleop_twist_keyboard teleop_twist_keyboard '''

now you can control the robot with keyboard
start by pressing i