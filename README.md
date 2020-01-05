# eezybotarm
ROS EEZYbotARM 

This repository is intended to contain software aimed at exploiting the eezybotarm robotic arm.
Attempting to create a urdf file that allows viewing and interacting with the model in rviz
The original project stls but with changed names are used.

https://www.thingiverse.com/thing:1015238 

https://www.instructables.com/id/EEZYbotARM/

git clone https://github.com/inaciose/eezybotarm.git

catkin_make

roslaunch eezybotarm rviz.launch model:=eezybotarm01.urdf