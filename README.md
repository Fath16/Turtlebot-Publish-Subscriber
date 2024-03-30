## About
To provide an understanding of how to create Robot by using URDF & RViz link_description.

## Requirement
- Ensure you're using Ubuntu version 20.04 
- Install ROS Noetic
- IDE Application such as Vs Code, PyCharm, Sublime…

## Instruction
- Clone or download the zip file of Link_description_HW5 branch repository
- Create catkin_ws folder in your local machine
- Copy the src folder from clone repository into catkin_ws
- Open terminal
- Build the catkin_ws by using this command
  
      cd ~/catkin_ws
      catkin_make
      
- Open new ternimal to lauch the simulation

      cd ~/catkin_ws
      source devel/setup.bash
      roslaunch twolink_description rviz.launch

- Check the simulation
