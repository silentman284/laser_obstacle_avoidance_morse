laser_obstacle_avoidance_morse
==============================
Author : Arkapravo Bhaumik (arkapravobhaumik@gmail.com) and Koushik Kabiraj (koushik.atti@gmail.com)

Laser obstacle avoidance in MORSE via ROS nodes
--------------------------------------------
To marry ROS Fuerte with MORSE 0.6 in Ubuntu 12.04 see these instructions, 
http://www.warp1337.com/content/morse-and-ros-detailed-installation-howto-ubuntu-precise

ROS fuerte prefix -- _/opt/ros/fuerte_  
MORSE prefix -- _/opt/ros/morse_

These simulations are for PR2 and ATRV, employing the SICK laser

1. Place the package in ROS PATH and build it
2. Place the files, _laser_obstacle_avoidance_morse/morse/atrv_laser.py_ and _laser_obstacle_avoidance_morse/morse/pr2_laser.py_ at _/opt/ros/morse/share/morse/examples/scenarii/_
3. Start an instance of the master
4. For PR2, start the MORSE simulation, _cd /opt/ros/morse/share/morse/examples/scenarii/ && morse run pr2_laser.py_ and start the ROS node, _roslaunch laser_obstacle_avoidance_morse obs_morse_pr2.launch_
5. For ATRV, start the MORSE simulation, _cd /opt/ros/morse/share/morse/examples/scenarii/ && morse run pr2_laser.py_ and start the ROS node, _roslaunch laser_obstacle_avoidance_morse obs_morse_atrv.launch_

PR2
-------------
![Image Alt](https://lh5.googleusercontent.com/-AKhCe3Tls6o/UUzefpEZjZI/AAAAAAAACZw/OC96MVG-WT0/s874/1.png)

ATRV
-------------
![Image Alt](https://lh6.googleusercontent.com/-7YZhCKeiokg/UUzeiipSy1I/AAAAAAAACZ4/WSOrYGjMXcU/s876/2.png)
