# Phase 2 Funding Proposal: Wrist Articulation and 6-DOF Integration

## 1. Project Objective
To construct the final three precision actuators required to complete the 6-DOF collaborative robotic arm. These units will form the "wrist" of the robot (controlling roll, pitch, and yaw), completing the kinematic chain and allowing for complex spatial manipulation.

## 2. Proof of Concept & Risk Mitigation
The hardware architecture has been successfully validated during the development of the 3-axis base. To reduce the moving mass at the end of the kinematic chain, these wrist axes utilize a scaled-down hardware architecture compared to the primary joints. This transitions the control from ODrive S1 controllers to the more compact ODrive Micro, and utilizes integrated motor units. Funding these components carries minimal risk as they seamlessly integrate into the established CAN FD communication network.

## 3. Bill of Materials (Requested Funding)
This request covers the electronics and mechanical drives for the three remaining wrist joints. Structural 3D printed components using PPA-CF have already been sourced independently.

* **3x ODrive Micro Motor Controllers**: $89.99 each, totaling $269.97. Specifications require Motor Controller for wrist actuators and 6th axis. The vendor is ODrive.
* **3x CubeMars GL60 Integrated Motors**: $108.99 each, totaling $326.97. Specifications require 4th, 5th, and 6th Axis motors. The vendor is CubeMars.

**Total Requested Funding for Phase 2: $596.94**
