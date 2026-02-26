## Members
Kian Kabir, Computer Engineering Student (2028)
KKabir@vt.edu

## Mentor
None

## Current Status
IN PROGRESS

## Project Overview

**6 Axis Collaborative Robot (Cobot)**

**Objective**

To design, build, and program a 6 axis robotic arm with a goal of achieving a 25 to 50 micron end effector repeatability with a 3kg payload. This is a robotic arm designed to achieve a high level of precision at a fraction of the overall cost associated with a traditional robotic arm. This robotic arm is designed to be highly safe around human operators through a decentralized CAN FD control architecture and advanced additive manufacturing techniques.

**System Architecture & Control**

This robotic arm is designed with a control architecture that allows for a bridge between path planning and ultra-low-latency motor commutation. A Raspberry Pi 5 is used to run ROS2 to calculate the inverse kinematics functions. However, due to the nondeterministic nature of a Linux OS, a 1 Mbps+ CAN FD bus is utilized to send target positions to six decentralized ODrive S1 controllers.

**Mechanical Design & Advanced Manufacturing**

Due to the need for micron accuracy while keeping the overall cost below $2,000, the mechanical structure is designed with a focus on minimizing rotational inertia through weight optimization:

Generative Design: The structural linkages have been optimized using generative CAD to remove unnecessary mass while preserving the critical load paths. This has greatly reduced the manufacturing time and material costs.

Engineering Grade Materials: The complex joint housing and motor mounts are fabricated using PPA-CF (Polyphthalamide Carbon Fiber), which provides extreme dimensional stability under both thermal and mechanical stress. The main arm spans are fabricated using roll-wrapped carbon fiber tubing.

**Human-Robot Interaction (HRI) & Safety**

As the robot will be used for human-robot collaboration, safety has been integrated at both the physical and software layers:

Proprioceptive Collision Detection: The robot will employ dual encoders (on the motor shaft and after the gearbox), which will continuously measure the mechanical delta. The moment it experiences any external force (such as a collision), it will detect the sudden change between the two sensors and stop operations immediately.

Kinematic Monitoring: The robot will be equipped with IMUs to monitor kinematics and detect sudden spikes in acceleration. The ODrive motor controllers will monitor the current draw to limit the absolute torque output during human interaction.



## Educational Value Added

This project is a complete and hands-on exploration of how to build a complex robot system from scratch. The project involves custom electronics development, enabling high-speed networking, and mixing software with physical hardware.

**Custom Electronics & Signal Integrity:** The project involves developing custom circuit boards for high precsion encoders. The primary objective of custom encoder development is to reduce cost as high resolution encoders capable of meeting this projects needs are extremely expensive. 

**High-Speed Networking:** The project involves setting up a robust and fast communication network (CAN FD), which enables the main computer to send simultaneous commands to all six motors of the robot arm at once with near zero latency.

**Applied Robotics Software:** The theoretical application of robotics software involves simulating the movements of the robot arm and then applying the same to the real world. The robotics software (ROS2) is developed to calculate the exact movements of the robot arm to reach a specific point in space. Learning how to use ROS2 in important as it can be used to control other industrial robots from established brands. 

**Smart Motor Control:** The motor controllers are developed to make corrections for physical deviations and use PID loops. Using PID loops the motor controllers have the ability to detect the flex of the robot arm and make corrections to maintain accuracy, and learning to tune these loops is extremely important.

## Tasks

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Design Decisions

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Design Misc

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Steps for Documenting Your Design Process

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## BOM + Component Cost

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Timeline

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Useful Links

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->

## Log

<!-- Your Text Here. You may work with your mentor on this later when they are assigned -->


