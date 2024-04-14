## Requirement
- Ensure you're using Ubuntu version 20.04 
- Install ROS Noetic
- IDE Application such as Vs Code, PyCharm, Sublime…

## Instruction
- Create catkin_ws folder in your local machine
- Create src folder
- Clone or download the zip file of Gazebo_MT branch repository into src folder
- Open terminal
- Build the catkin_ws by using this command
  
      cd ~/catkin_ws
      catkin_make
      
## Test the simulation
Open terminal: 

    source devel/setup.bash

Rviz:

    roslaunch rrbot_description rrbot_rviz.launch

Gazebo:

    roslaunch rrbot_gazebo rrbot_world.launch


- Link to youtube

      https://youtu.be/YktJKEEcgQw





