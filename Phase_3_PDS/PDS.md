# Power Distribution System (PDS) Funding Proposal

## 1. Project Objective
To construct the Power Distribution System (PDS) responsible for safely powering the 6-DOF robotic arm. This system will step down AC mains power to supply the high-current 48V motor bus, the 24V auxiliary logic loop, and the 5.1V logic power for the central compute system.

## 2. Proof of Concept & Risk Mitigation
The electrical architecture incorporates standard industrial safety practices, including a critical hardware Emergency Stop (E-Stop) loop. This loop is designed to instantly sever motive power to the high-voltage motor controllers without cutting logic power to the central compute unit, ensuring the system can safely log faults and maintain telemetry during an emergency event. Utilizing proven standard industrial relays and contactors guarantees a robust and reliable power delivery system.

## 3. Bill of Materials (Requested Funding)
This request covers the power supplies, contactors, relays, and distribution blocks required for the electrical cabinet and safety loop.

* **1x Meanwell HRPG-1000N3-48 Power Supply**: $220.40 each, totaling $220.40. Specifications require a 1000W (3200W peak) supply to drive the main 48V bus. The vendor is Mouser Electronics.
* **1x Meanwell LRS-350-24 Power Supply**: $31.40 each, totaling $31.40. Specifications require a 350W supply to power the 24V auxiliary bus for contactor coils and relays. The vendor is DigiKey.
* **1x 5.1V LFWLT40-1000 Power Supply**: $27.30 each, totaling $27.30. Specifications require clean 5.1V logic power for the compute system. The vendor is DigiKey.
* **1x RECT0P1CX Contactor**: $33.00 each, totaling $33.00. Specifications require a 48V rating to physically break the high-voltage bus. The vendor is DigiKey.
* **1x 19AS1D12-48 Relay**: $8.10 each, totaling $8.10. Specifications require a 24V rating for the E-Stop circuit logic handling. The vendor is DigiKey.
* **1x ECS-30RE1RM2Q-100Q Mushroom Button**: $5.95 each, totaling $5.95. Specifications require a hardware interrupt trigger for the E-Stop. The vendor is DigiKey.
* **10x Wago 5-Terminal Connectors**: $1.68 each, totaling $16.80. Specifications require quick-disconnect terminal blocks for routing power. The vendor is DigiKey.

**Total Requested Funding for PDS: $342.95**
