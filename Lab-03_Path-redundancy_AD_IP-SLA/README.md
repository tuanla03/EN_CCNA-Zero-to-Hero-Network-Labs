# Lab-03: \[Path redundancy with AD & IP SLA]


## 1. Topology Diagram

[Network Topology](topology_lab-03.png)


## 2. Lab Objectives

* Administrative Distance (AD) configuration.

* IP SLA (Service Level Agreement) configuration.

* Link the IP SLA state to a static route via Track to enable automatic path switching.


## 3. IP Addressing Table

| Device | Interface | IP Address | Subnet Mask |
| :---: | :--- | :--- | :---: |
| R1 | e0/0 | 192.168.1.1 | /24 |
| R1 | e0/1 | 192.168.12.1 | /24 |
| R1 | e0/2 | 192.168.13.1 | /24 |
| R1 | e1/0 | 192.168.15.1 | /24 |
| R1 | e1/1 | 192.168.51.1 | /24 |
| R2 | e0/0 | 192.168.24.1 | /24 |
| R2 | e0/1 | 192.168.12.2 | /24 |
| R3 | e0/1 | 192.168.34.1 | /24 |
| R3 | e0/2 | 192.168.13.2 | /24 |
| R4 | e0/0 | 192.168.24.2 | /24 |
| R4 | e0/1 | 192.168.34.2 | /24 |
| R4 | e0/2 | 192.168.4.1 | /24 |
| R5 | e0/0 | 192.168.15.2 | /24 |
| R5 | e0/1 | 192.168.51.2 | /24 |
| R5 | e0/2 | 192.168.5.1 | /24 |
| VPC1 | eth0 | 192.168.1.2 | /24 |
| VPC4 | eth0 | 192.168.4.2 | /24 |
| VPC5 | eth0 | 192.168.5.2 | /24 |


## 4. Configuration Highlights

n/a

*To view full configurations, please check the `/configs` folder.*


## 5. Verification Commands

Use these commands to verify the lab status:

show ip route - View the entire routing table.

show ip route static - View specifically the static route in routing table.

show ip interfaces brief - View the IP address of the respective interfaces.

ping (IP Address) - Verify the connection between devices.

traceroute (IP Address) - Track the paths of your packet take to reach the destination.
