# Lab-05: \[Router on a Stick]


## 1. Topology Diagram

[Network Topology](topology_lab-05.png)


## 2. Lab Objectives

* Inter-VLAN Routing: Configure router to route traffic between different VLANs using a single physical interface on a Router.


## 3. IP Addressing Table

| Device | Interface | IP Address | Subnet Mask |
| :---: | :--- | :--- | :---: |
| R1 | e0/0 | 192.168.1.1 | /24 |
| R1 | e0/0.2 | 192.168.2.1 | /24 |
| R1 | e0/0.3 | 192.168.3.1 | /24 |
| VPC1 | eth0 | 192.168.1.2 | /24 |
| VPC2 | eth0 | 192.168.2.2 | /24 |
| VPC3 | eth0 | 192.168.3.2 | /24 |


## 4. Configuration Highlights

On the Router: Create sub-interfaces and assign encapsulation for each VLAN by standing at Interface Config Mode and type:
* encapsulation dot1q (VLAN id)
* ip address (ip address) (subnet mask)

*To view full configurations, please check the `/configs` folder.*


## 5. Verification Commands

Use these commands to verify the lab status:

show vlan - View the VLANs and check the VLAN that assign with each ports.

show interfaces trunk - View the interfaces that configured as a trunk port and VLANs that port allow.

ping (IP Address) - Verify the connection between devices.
