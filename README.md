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







