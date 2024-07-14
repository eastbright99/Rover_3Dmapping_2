# Updates with Rover
## Projects detail (continuing from previous EGG-499)
* Department : UNLV Electrical and Computer Engineering  
* Place : SEB #3229  
* Duration : 01/16/24 ~ 01/24/24  
* Updates : structures, inside, system setup  

<br/><br/><br/>

# Hardware
## Structure
### Design 3D modeling
* with Blender
<img src="./images/01.png" width="600" height="330"/> 
<img src="./images/02.png" width="600" height="330"/> 

<br/>

### Print
* with Flsun superracer
<img src="./images/03.jpg" width="200" height="350"/> 

<br/>

### Assemble
* Lidar plate and stand  
<img src="./images/04.png" width="400" height="600"/>

* Camera holder

<img src="./images/05.png" width="200" height="200"/><img src="./images/06.png" width="200" height="200"/>

* Inner plate and stand

<img src="./images/07.png" width="300" height="400"/><img src="./images/08.png" width="300" height="400"/> 

<br/><br/><br/>

## Inside
* wiring and placing stuffs

<img src="./images/09.png" width="300" height="400"/><img src="./images/10.png" width="300" height="400"/>

<br/><br/><br/>

# Software
## Main system files
* /etc/systemd/system/roverrobotics.service  
<img src="./images/11.png"/>

* /usr/sbin/roverrobotics  
<img src="./images/12.png"/>

* /etc/roverrobotics/env.sh  
<img src="./images/13.png"/>  

<br/><br/><br/>

## Main workspaces function
<img src="./images/14.png"/>  

* catkin_ws : rover driver  <br/>
* realsense_ws : camera and imu transform  <br/>
* velodyne_ws : pointcloud  <br/>
* liosam_ws : mapping  <br/>

<br/><br/><br/>

## IP setup for ssh
* /etc/roverrobotics/env.sh 
* ~/.bashrc

<br/><br/><br/>

## Velocity setup
* roverrobotics_ros_driver.cpp  
<img src="./images/15.png"/>  

<br/><br/><br/>

# Results
## Looks
<img src="./images/16.png" width="300" height="300"/><img src="./images/17.png" width="300" height="300"/>  
<img src="./images/18.png" width="300" height="300"/><img src="./images/19.png" width="300" height="300"/>  

<br/><br/><br/>

## Test
[Test Vid](https://youtu.be/PPUc6Rkc0Pk)  

<br/><br/><br/>

## Map result
<img src="./images/20.jpg" width="400" height="400"/>

<br/><br/><br/>

## Discussion
During this project, I studied ROS thoroughly and gained a comprehensive understanding of both the hardware and software components of robots. By utilizing camera and implementing depth cloud processing, I was able to identify gaps in the environment and perceive the surroundings more accurately. Also, integrating a rover with LIDAR, I successfully obtained 3D data and created detailed maps of the environment. Although I couldn't implement a navigation function in this particular project, I successfully achieved it in a previous project, Mobile Robotics.

<br/><br/><br/>
