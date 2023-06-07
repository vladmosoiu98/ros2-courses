# ros2-courses
Resources to start working with ROS2

# Official documentation
The official documentation for ROS2 Humble has a very good structure, but becomes understandable mostly when you already have some brief ideas about ROS. 
Hence, I would recommend first some video tutorials to get some brief ideas before digging in the codes and the detailed explanation provided in the docs.
Link: https://docs.ros.org/en/humble/index.html

### Installation on Ubuntu 22.04
Command line installation (make sure to installl the desktop version and the dev-tools)
Link: https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debians.html

---

# Video Tutorials
Some of the greatest resources for ROS are the following channels:
- Articulated Robotics : https://www.youtube.com/@ArticulatedRobotics
- Robotics Back-End : https://www.youtube.com/@RoboticsBackEnd
Those two go from the most basic concepts of ROS and into some nice details about the sensors or more complex parts, such as navigation and perception.

---

# Roadmap
Once you get the ideas behind ROS (even as briefly as possible), this is just a reference, might as well try it any way you want:
1. Nodes and topics - those are teh fundamentals of ROS, once you get to understand how they work individually and together, you already have the tools to start building
2. Packages - the nodes are usually placed in them, plus they provide the modularity of ROS so it is an important aspect to understand
3. colcon command - this is used to compile the packages (both Cpp and Python) and binds them based on the dependencies
4. URDF (Unified Robotics Description Format) - this is the structure that defines your robot, you can still go into programming with ROS without it, but at some point you will have to deal with it and its structure

---

## Tips
### Sourcing
Don't forget to SOURCE both the ROS distribution ("source /opt/ros/humble") and the install of your project ("source install/setup.bash")!!!
For the first sourcing, its better if you add the command in the ~/.bashrc file (this way every time you open a terminal it automatically does it).
That can be done through:
```
 echo "source /opt/ros/humble" >> ~/.bashrc
```
### ROS Domain ID
At some point you will work on the same netwrok with multiple persons doing different things. 
This is quite far away from the beginning but its important. The ROS Domain ID is an unique identifier.
```
echo "export ROS_DOMAIN_ID=<your_domain_id>" >> ~/.bashrc
```
