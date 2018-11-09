# ROS (Robotics Operating System) install on raspberry pi
### Hardware requirement
- Raspberry pi 2/3
- SD card 16 GB to 32 GB
- Card reader
- HDMI monitor (optional)
- Keyboard (optional)
- Mouse (optional)
     
## Download
 **Download ROS Image (Ubuntu mate)**
- https://downloads.ubiquityrobotics.com/pi.html
- It take some minutes about 1 GB file. When download completed Unzip ROS image into a folder 

 **Download Win32DiskImager**
- https://drive.google.com/file/d/1Bs2cClNa-LKqeoK8Kmcm-DWhFKsQw2dj/view?usp=sharing 
- when download complete then install Win32DiskImager
- Open Win32DiskImager 
## Image write into SD Card
- Inser SDCard into your pc
- Open Win32DiskImager
![alt text](diskimage.png)
- Set image path using red circle button
- **Select SDcard using green circle
- **Everything is ok then click write
- **It will takes some minutes

## Start ROS operating system
- Insert SDcard into Raspberry pi
- Power up
- Psername: **ubuntu**
- Password: **ubuntu**
## Test ROS
- Press **Ctrl+Alt+T** for open terminal
- **Open terminal** 
## Test    
               
    $ rostopic list
    Output
    /battery_state
    /cmd_vel
    /diagnostics
    /joint_states
    /joy
    /left_error
    /motor_node/parameter_descriptions
    /motor_node/parameter_updates
    /right_error
    /rosout
    /rosout_agg
    /statistics
    /tf
    /tf2_web_republisher/cancel
    /tf2_web_republisher/feedback
    /tf2_web_republisher/goal
    /tf2_web_republisher/result
    /tf2_web_republisher/status
    /tf_static
    
    
    
### Thanks install Completed    

## Creating a catkin Package

You have already **catkin_ws** this Workspace

    $ ls
    output 
    catkin_ws  Desktop  Documents  Downloads  Music
## Creating a catkin Package
    
    $ cd catkin_ws/src     
    $ catkin_create_pkg beginner_tutorials std_msgs rospy roscpp
    $ cd
    
## Building a catkin workspace and sourcing the setup file    

    $ cd catkin_ws/
    $ catkin_make
    
