## Run ROS    
    $ roscore
## Run turtlesim
    $ rosrun turtlesim turtlesim_node
## turtle keyboard teleoperation
    $ rosrun turtlesim turtle_teleop_key
## Run  rostopic for echo
    $ rostopic echo /turtle1/cmd_vel
## Run Graph
    $ rosrun rqt_graph rqt_graph    
## ROS Hydro and later
forward-left circle
     
     $ rostopic pub -1 /turtle1/cmd_vel geometry_msgs/Twist -- '[2.0, 0.0, 0.0]' '[0.0, 0.0, 1.8]'   
## Looping   ROS HYDRO
    $ rostopic pub /turtle1/cmd_vel geometry_msgs/Twist -r 1 -- '[2.0, 0.0, 0.0]' '[0.0, 0.0, -1.8]'   
    
## Show position

    $ rostopic echo /turtle1/pose       
http://wiki.ros.org/ROS/Tutorials/UnderstandingTopics




[Reference](http://wiki.ros.org/ROS/Tutorials)             