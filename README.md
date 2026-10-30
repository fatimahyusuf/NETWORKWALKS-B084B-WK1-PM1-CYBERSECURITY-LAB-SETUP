# NETWORKWALKS-B084B-WK1-PM1-CYBERSECURITY-LAB-SETUP
# 🔐Cybersecurity Lab Environment Setup

Building an isolated virtual lab for penestration testing and ethical hacking pratices

# 🎯Project Overview

This project involves building a virtual cybersecurity lab using VirtualBox and Kali Linux to practice penetration testing and explore various cybersecurity techniques.

The lab provides a safe and isolated environment for carrying out activities such as network scanning, reconnaissance, vulnerability identification, and security testing. It is designed to support hands-on learning and allow these exercises to be repeated whenever necessary.

A private virtual network is used to connect the lab environment, making it possible to introduce additional virtual machines in the future for authorized testing and practical cybersecurity experiments.

# 🎯 Project Objectives 

- Install and configure VirtualBox and Kali Linux.
- Set up a private NAT Network for the lab.
- Configure and verify Kali Linux network connectivity.
- Assign a stable IP address to the virtual machine.
- Create a recovery snapshot.
- Document the setup process and prepare the lab for future cybersecurity activities.

# Lab Configuration 

| Component              | Configuration    |        
|------------------------|------------------|
| Virtual platform       | Oracle VirtualBox 7.2.6 |
| Primary Security VM    | Kali Linux 2026.2           |
| Network Type           | NATNetwork                   |
| Network Address        | 10.0.0.0/24                  |
| Network Name           | NatNetwork                   |
| Kali Interface         | eth0                         |
| Kali IP Address        | 10.0.0.2/24                  |
| Default Gateway        | 10.0.0.1                     |
| DNS Server             | 8.8.8.8                      |

# 🪜Lab Setup Procedures 

## Step 1- Install Oracle VirtualBox 

Oracle VirtualBox 7.2.6 was successfully installed and set up to serve as the virtualization platform for the cybersecurity lab.
## VirtualBox Installation 
<img width="780" height="615" alt="Screenshot 2026-10-30 132540" src="https://github.com/user-attachments/assets/fb3d3cbb-9ee5-4e48-b168-3f853ca78fb4" />


## Step 2- Install Kali Linux 

Kali Linux 2026.2 was deployed as the main virtual machine for the lab, providing the platform for running cybersecurity tools and performing ethical hacking exercises.
## Kali Linux Installation 
<img width="802" height="33" alt="Screenshot 2026-10-30 134952" src="https://github.com/user-attachments/assets/0d235835-db60-40b1-a2ad-0fdf1a548033" />
<img width="612" height="502" alt="Screenshot 2026-10-30 135054" src="https://github.com/user-attachments/assets/7e29f219-92f5-4cc8-b799-dbc40305e959" />



## Step 3- Configure the Virtual Network 

A dedicated NATNETWORK was assigned in VirtualBox 

```text
Configuration 
Network Name: NatNetwork 
IPv4: 10.0.0.0/24
DHCP: Enabled 
IPv6: Disabled
````
## Virtual Network Configuration 
<img width="1910" height="966" alt="Screenshot 2026-10-30 140955" src="https://github.com/user-attachments/assets/74572f6a-1c84-4611-aaaa-732c1f1303e3" />


## Step 4- Import Kali Linux 

The Kali Linux virtual machine was extracted and successfully added to Oracle VirtualBox.


## Step 5- Configure the Kali Linux Network 

The Kali Linux network interface eth0 was configured for the laboratory network 
## Network Configuration 
```text
IP Address: 10.0.0.2
Netmask:    24
Gateway:    10.0.0.1
DNS:        8.8.8.8
```
      
## Kali Linux Network Configuration 
<img width="1047" height="695" alt="Screenshot 2026-10-30 142122" src="https://github.com/user-attachments/assets/a08e79db-4347-48d4-85aa-b079645e1833" />

## Verification Commands 
```text
ip link show eth0
ip a
ip route
nmcli device status
```
These commands were used to verify the interface status, ip address, routing information and NetworkManger Status.

## Step 6- Create a Clean Virtual Machine Snapshot

A baseline snapshot was saved after completing the initial Kali Linux setup.
This serves as a backup point, allowing the lab environment to be restored whenever needed during future cybersecurity activities.
## Clean Virtual Machine Snapshot
<img width="1903" height="919" alt="Screenshot 2026-10-30 142603" src="https://github.com/user-attachments/assets/91806929-10cf-4d8e-ae50-6c864e724f1f" />

# What I Learned

This project provided practical experience in building and managing a virtual environment for cybersecurity testing.

The key concepts and skills gained include:

### 1. Static IP Configuration
I learned how to assign and verify static IP addresses, subnet masks, default gateways, and DNS settings in Kali Linux.

### 2. Virtual Machine Snapshots
I learned the importance of creating baseline snapshots to preserve a working environment and provide a recovery point before future experiments.

### 3. Technical Documentation
I developed practical documentation skills by recording configurations, commands, screenshots, challenges, and solutions throughout the project.

# Security and Ethical use 
This laboratory is intended strictly for education purposes only.




