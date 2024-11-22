# Go Chase It Project

## Project Description
The "Go Chase It" project involves designing a ball-chasing robot using ROS (Robot Operating System), Gazebo, and C++. The goal of this project is to create a differential drive robot that can chase a white ball within a simulated environment. The robot is equipped with sensors, including a lidar and a camera, to detect the ball and navigate towards it. This project combines various robotics concepts, including robot modeling, sensor integration, and control algorithms.

## Packages and Algorithms Used
- **ROS (Robot Operating System)**: A flexible framework for writing robot software. It provides tools and libraries to help build robot applications.
- **Gazebo**: A powerful robot simulation tool that allows for the creation of complex environments and interactions.
- **C++**: The primary programming language used to implement the robot's control logic and sensor processing.
- **Lidar and Camera Sensors**: Used for detecting the environment and locating the white ball.
- **Gazebo Plugins**: Used to integrate the robot's differential drive, lidar, and camera with the Gazebo simulation.

## Project Structure
project_directory/ 

    ├── my_robot/ 
    │ ├── urdf/ 
    │ │ └── my_robot.xacro 
    │ ├── launch/ 
    │ │ ├── world.launch 
    │ │ └── robot_description.launch 
    │ └── src/ │ ├── drive_bot.cpp 
    │ └── process_image.cpp 
    └── ball_chaser/ 
    ├── src/ 
    │ ├── command_robot.cpp 
    │ └── process_image.cpp 
    └── CMakeLists.txt


## Steps to Run the Project

1. **Install Dependencies**:
   Ensure that you have ROS and Gazebo installed on your system. Follow the installation instructions from the [ROS website](http://wiki.ros.org/ROS/Installation) and the [Gazebo website](http://gazebosim.org/).

2. **Clone the Repository**:
   Clone your project repository to your local machine:
   ```bash
   git clone <repository_url>
   cd project_directory

3. **Build the Project**: Navigate to the project directory and build the project using catkin_make:

        cd ~/catkin_ws
        catkin_make

4. **Source the Workspace**: Source the workspace to ensure ROS can find your packages:

        source devel/setup.bash

5. **Launch the Gazebo Simulation**: Launch the world that includes the robot and the white ball:

        roslaunch my_robot world.launch

6. **Run the Robot Control Nodes**: In a new terminal, run the drive_bot and process_image nodes:

        roslaunch ball_chaser ball_chaser.launch

**Conclusion**

The "Go Chase It" project showcases my ability to design and implement a robotic system that can interact with its environment. This project serves as a practical application of robotics concepts and prepares you for more advanced robotics challenges.
