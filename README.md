# TASK-4
: Configure and test basic firewall rules to allow or block traffic
 #  Basic Firewall Configuration and Testing

##  Objective

This Task demonstrates how to configure and test basic firewall rules to allow or block traffic.

-  UFW (Uncomplicated Firewall) on Linux.

# What I Have Learned

Through this exercise of configuring and testing basic firewall rules using Windows Firewall and UFW on Linux.

1. Understanding Firewall Basics
 
     A firewall acts as a security barrier that controls incoming and outgoing network traffic.

     Rules can be set to allow or block specific ports, IP addresses, or protocols based on security needs.

2. Using UFW on Linux

     Learned how to enable, disable, and reset UFW — the default firewall tool on many Linux distributions.

     Practiced commands to allow (e.g., SSH port 22) and deny (e.g., HTTP port 80) network traffic.

     Used ufw status verbose to review current rules clearly.

  ##  Tools Used

- **UFW** – Uncomplicated Firewall (default in many Linux distros like Ubuntu, parrot os, kali linux.)

 #  Tasks Completed
  ###  UFW on Linux: Allow SSH (port 22) and Deny HTTP (port 80)

#  Commands Used:

## Enable UFW
sudo ufw enable

### Allow SSH (port 22)
sudo ufw allow ssh

## Deny HTTP (port 80)
sudo ufw deny 80

## Check firewall status
sudo ufw status verbose

# Screenshots for enabling the UFW :

<img width="1366" height="601" alt="Screenshot at 2025-08-08 18-27-18" src="https://github.com/user-attachments/assets/8705e6dd-5e02-49b3-9b41-5332d79d24a5" />

<img width="1366" height="601" alt="Screenshot at 2025-08-08 18-26-49" src="https://github.com/user-attachments/assets/09b41375-cb6b-4837-93f2-018d8985c256" />

# Remove Test Rules - UFW(Linux) 

sudo ufw delete deny 80

# Screenshots for disabling the UFW : 

<img width="594" height="306" alt="Screenshot at 2025-08-08 18-29-46" src="https://github.com/user-attachments/assets/11a55962-696b-40d4-9366-c6642792503d" />

#Testing the Rules

## Method:

Use curl (Test connectivity to the web server) 

Port 80 (HTTP) should be blocked

Port 22 (SSH) should be accessible if applicable

 # Summary - Firewall Filters Traffic 
 
A firewall is a network security system that monitors and controls incoming and outgoing traffic based on predefined rules. Its main purpose is to allow safe traffic and block potentially harmful traffic.
## 1.Traffic Inspection

Every packet of data entering or leaving a system is inspected by the firewall.

## 2.Rule Matching

The firewall checks each packet against a set of rules defined by the user or system.

Port number (e.g., block port 80)

IP address (e.g., allow only from 192.168.1.1)

Protocol (e.g., allow only TCP, block UDP)

Direction (inbound or outbound)

## 3.Decision Making

 For each packet, the firewall decides to:

 Allow it (if it matches an “allow” rule)

 Deny/Block it (if it matches a “deny” rule or no rules apply)

# Conclusion : 

This project demonstrates how to apply and verify basic firewall rules using Windows Firewall and UFW. Testing with curl confirmed that rules worked as intended — blocking or allowing specific traffic.

  
