# AI-and-data-science-task4
Install and use the turtlesim package

# Background
 This project documents learning the fundamentals of ROS 2 (Robot Operating System) using the Turtlesim visual simulator. 
It starts with creating an account on The Construct website to obtain a ready-to-use virtual development environment for learning ROS without the need for local installation.

# Project Goals
- Understand the theoretical and practical basics of the ROS 2 system.
- Get to know the ROS 2 Humble development environment.
- Learn how to run and play around with the Turtlesim simulator.
- Grasp the basic concepts in ROS 2 like Nodes, Topics, and Actions.

# Prerequisites
- An account on (https://www.theconstruct.ai/)
- ROS 2 Humble environment (available on The Construct)

# Implementation Steps
1. **Create an Account on The Construct**:
   - Log in to the virtual environment
2. **Set Up the Project**:
   - Go to the "ROSjects" section
   - Select the ROS 2 Humble environment
   - Open the virtual environment and terminal

3. **Running Turtlesim**:
   - Execute the following commands in the terminal:
     ```bash
     # Update the environment
     source /opt/ros/humble/setup.bash
     # Run Turtlesimros2
     run turtlesim turtlesim_node
    - Open a new terminal and run:
      ```bash
      # Run the turtle control
      ros2 run turtlesim turtle_teleop_key
  4. **Basic Concepts in ROS 2**:
     
  - (Nodes) Nodes are independent processes that perform computational tasks. In ROS 2, each node is responsible for a specific function in the system. In the Turtlesim project, we have two main nodes:
    
       - `turtlesim_node`: displays the visual window and controls the turtle's movement.
         
       - `teleop_turtle`: reads keyboard inputs and sends them to the other node.
       
 - (Topics) Topics are communication channels used to send data between nodes in a publish-subscribe model.  In Turtlesim:
   
       - `/turtle1/cmd_vel` : a topic for publishing speed commands for the turtle.
   
       - `/turtle1/pose` : a topic that publishes information about the turtle's position and speed.
       
 - (Actions) Actions are a communication pattern used for long-running tasks that need feedback and results. They consist of:
   
       - Goal: the objective to be achieved.
   
       - Feedback: updates on the progress of the task.
   
       - Result: the final outcome when the task is complete.
   
  5. **The sources**:
     - https://www.youtube.com/watch?v=e_MSlH0YIyA
     - https://docs.ros.org/en/humble/Tutorials/Beginner-CLI-Tools/Introducing-Turtlesim/Introducing-Turtlesim.html
