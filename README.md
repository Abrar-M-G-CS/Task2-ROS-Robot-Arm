# Task2-ROS-Robot-Arm
ROS packages to control an Arduino robot arm by using Moveit 

In this task we had to install the ROS packages to control the robot arm , unfortuently i had multiple problems during the installation and i have included it in the output file i have tried to find mutilpe solutions on youtube , but still it didnt work , i might reinstall the whole linux system and reinstall ROS operating system and try to add more memory  

I have included the steps that worked with me and the step that failed to work 

the first step was to run the depndencies from the arduino_robot_arm 

$ rosdep install --from-paths src --ignore-src -r -y

then i had to install the rest of the packages , since i have the noetic distro i had to run these commands: 

$ sudo apt-get install ros-noetic-moveit
$ sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui
$ sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher
$ sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control

the problem that happend with me was i coud install the first 3 commands then the last one an error occurs that states the following 

E: You don't have enough free space in /var/cache/apt/archives/. 

i have included the output in the output file 
