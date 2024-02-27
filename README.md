# Turtlebot-Publish-Subscriber
## About
To provide an understanding of how to create and run the code of drawing turtle_cycle.

## Requirement
- Ubuntu
- Install of ROS Noetic
- IDE Application such as Vs Code, PyCharm, Sublime…

## Instruction
**Step One**
- Open IDE
- Create package python script 
- Include this script into the file
  
      import rospy
      from geometry_msgs.msg import Twist
      import sys
      
      def move_turtle(line_vel, ang_vel):
         rospy.init_node('turtlemove', anonymous=True)
         pub  = rospy.Publisher('/turtle1/cmd_vel', Twist, queue_size=10)
         rate = rospy.Rate(10)
      
      
         vel = Twist()
      
      
         while True:
             vel.linear.x= line_vel
             vel.linear.y= 0
             vel.linear.z= 0
      
      
             vel.angular.x= 0
             vel.angular.y= 0
             vel.angular.z= ang_vel
      
      
             pub.publish(vel)
             rate.sleep()
  
      
      move_turtle(3.0, 2.5)
  
- Save the file in specific directory

**Step Two**
- Initialize source
- Run command in terminal

      source /opt/ros/noetic/setup.bash
      roscore
  
**Step Three**
Open another terminal and run

    rosrun turtlesim turtlesim_node

**Step Four**
- Open another terminal
- locate the spcific directory

      cd specific folder
  
- run the python file

      python3 file_name.py
    
  




