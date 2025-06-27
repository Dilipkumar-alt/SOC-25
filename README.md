# SOC-25
Autonomous Navigation of Robots
Initially we gone through Research Project.(https://github.com/MickyasTA/DRL_robot_navigation_ros2?tab=readme-ov-file)

The project's goal is to use Deep Reinforcement Learning (DRL) in the ROS2 (Robot Operating System 2) framework to create a mobile robot navigation system that can function on its own. The Twin Delayed Deep Deterministic Policy Gradient (TD3) algorithm is used to teach the robot to avoid obstacles in a simulated environment. The project consists of:

Pipelines for DRL training  
Communication between ROS2 nodes  
Gazebo simulation; mapping using SLAM; and testing autonomous behavior in real time  

2. Work Completed Thus Far  
A. Examining the Repository  
I studied the structure of the entire GitHub repository and became familiar with the project's workflow. 
I determined how the TD3 algorithm works in a simulation environment that is compatible with ROS2. 
I was aware of how different files, such as launch files, map files, and SLAM integration, contribute to the system.

B. ROS2 + DRL System Understanding  
I grasped how ROS2 nodes interact, including how sensory data like LIDAR is collected and how velocity commands are published.  
I explored how slam_toolbox is used for real-time mapping during robot navigation.  
I learned about launch file configurations and how Gazebo works with ROS2 to create a real-world simulation.  

C. Learning the DRL Pipeline  

I studied the TD3 algorithm and why it’s effective for continuous control tasks like navigation.  
I observed training issues, such as poor exploration due to a static simulation, and noted the use of pre-trained models to help with convergence challenges.  
I gained insights into how policy networks (actor-critic) are structured in DRL and how reward signals guide learning.  

3. Key Learnings
   
ROS2 Workflow: I learned about installation, workspace setup, ROS2 launch files, node composition, and simulation integration using Gazebo. 
TD3 Algorithm: I found out how TD3 improves on DDPG by using twin critics, delayed updates, and noise smoothing for better training in continuous action spaces.  
Simulation Challenges: I realized the importance of randomization in training environments and how even small changes, like shuffling obstacle positions, can affect DRL results.  
SLAM Integration: I understood how real-time mapping works with slam_toolbox and why setting global goals is important for long-range navigation.  
Code Architecture: I learned how ROS2 packages are structured and the value of a modular, reusable design when working with robotic systems.  
Debugging DRL Failures: I needed to closely monitor Q-value drops and understand the reasons for non-convergence, requiring a solid grasp of reinforcement learning concepts.  

5. Plan Ahead 

I aim to integrate a global planner to guide the robot more intelligently, moving beyond just obstacle avoidance.  
Currently beginning to work on the current personal project of ours.

I also intend to contribute better documentation or modular enhancements to the existing repository for improved community use.  

6. Final Thoughts  
This project has given me a practical chance to apply my theoretical knowledge of reinforcement learning in real robotics using ROS2. It has deepened my understanding of simulation, control systems, robot autonomy, and the real challenges of applying DRL in changing environments. The combination of system-level knowledge and algorithmic detail has made this experience very rewarding so far.
