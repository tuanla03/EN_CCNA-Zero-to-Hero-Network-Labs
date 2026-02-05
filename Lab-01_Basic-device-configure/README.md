# Lab-01: \[Basic device configure]


## 1. Topology Diagram

![Network Topology](topology_lab-01.png)


## 2. Lab Objectives

* Navigating between different configuration modes, including User EXEC, Privileged EXEC, and Global Configuration.

* Assign names to devices for easier identification.

* Configure a console password and encrypt it to ensure passwords are not visible in the running configuration.


## 3. IP Addressing Table

| Device | Interface | IP Address | Subnet Mask |
| :---: | :--- | :--- | :---: |
| R1 | e0/0 | 192.168.1.1 | /24 |
| VPC1 | eth0 | 192.168.1.2 | /24 |


## 4. Configuration Highlights

*To view full configurations, please check the `/configs` folder.*


## 5. Verification Commands

Use these commands to verify the lab status:

show ip interfaces brief - View the IP address of the respective interfaces.

ping (IP Address) - Verify the connection between devices.
