# eezybotarm ROS
ROS for EEZYbotARM MK1 and MK2

This repository is intended to contain software aimed at exploiting the eezybotarm robotic arms on ROS. 

EEZYbotARM MK1 and MK2 are modeled after the ABB IRB460 industrial grade robotic arm. 

Urdf file that allows viewing and interacting with the model in rviz.

The kinematic chain of the IRB460 is closed loop so in order to be visualized in RViz, the kinematic chain model must be converted to an
equivalent group of open-loop chains. The joint angles from the open-loop equivalent chains will then be used back to
control the visualized model in RViz in order for it to properly display the correct configurations given the joint angles 

For the MK2 model I found that the conversion and the URDF is already done, and available at: https://github.com/HotBlackRobotics/ntbd
For the MK1 model was done based in the MK2 urdf but with cylinders and boxes instead of meshes.


# EEZYbotARM MK1

https://www.thingiverse.com/thing:1015238 

https://www.instructables.com/id/EEZYbotARM/

http://www.eezyrobots.it/eba_mk1.html

# EEZYbotARM MK2

https://www.thingiverse.com/thing:1454048

https://www.instructables.com/id/EEZYbotARM-Mk2-3D-Printed-Robot/

http://www.eezyrobots.it/eba_mk2.html


# SETUP AND RUN 

cd ~/catkin_ws/src

git clone https://github.com/inaciose/eezybotarm.git

catkin_make

Lançar visualização do EEZYbotARM MK1

roslaunch eezybotarm rviz1.launch

Lançar visualização do EEZYbotARM MK1

roslaunch eezybotarm rviz2.launch
