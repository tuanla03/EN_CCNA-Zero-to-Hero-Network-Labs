# Lab-06: \[Switch Virtual Interface]


## 1. Topology Diagram

[Network Topology](topology_lab-06.png)


## 2. Lab Objectives

* Inter-VLAN Routing with SVI: Replace Router by a Multilayer Switch (Layer 3 Switch), configure virtual interface (SVI) to act as the default gateway.


## 3. VLAN database

| VLAN ID | VLAN Name | IP Address |
| :---: | :--- | :---: |
| VLAN 1 | IT | 192.168.1.1/24 |
| VLAN 2 | Sales | 192.168.2.1/24 |
| VLAN 3 | Guest | 192.168.3.1/24 |


## 4. IP Addressing Table

| Device | Interface | IP Address | Subnet Mask |
| :---: | :--- | :--- | :---: |
| VPC1 | eth0 | 192.168.1.2 | /24 |
| VPC2 | eth0 | 192.168.2.2 | /24 |
| VPC3 | eth0 | 192.168.3.2 | /24 |


## 5. Configuration Highlights

* ip routing - enable routing on a switch
* interface vlan (VLAN id) - create virtual interface for routing

*To view full configurations, please check the `/configs` folder.*


## 6. Verification Commands

Use these commands to verify the lab status:

show vlan - View the VLANs and check the VLAN that assign with each ports.

show ip route

ping (IP Address) - Verify the connection between devices.
