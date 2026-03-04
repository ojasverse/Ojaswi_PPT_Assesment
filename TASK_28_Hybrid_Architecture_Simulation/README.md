# Task 28 - Hybrid Architecture Simulation

# Objective
To simulate secure hybrid cloud architecture using:
- VPC
- Public & Private Subnets
- Bastion Host
- Route Tables
- Security Groups

# Architecture Design
sUser - Bastion Host - Private VM  
The Bastion Host acts as a jump server to securely access the private instance.
Private VM is NOT directly accessible from the internet.


# Implementation Steps
1. Created VPC
- CIDR: 10.0.0.0/16
- DNS Enabled

2. Created Subnets
- Public Subnet: 10.0.1.0/24
- Private Subnet: 10.0.2.0/24

3. Created Internet Gateway
- Attached to VPC
- Associated with Public Route Table

4. Configured Route Tables
Public:
- 0.0.0.0/0 - Internet Gateway

Private:
- No Internet Gateway attached

5. Launched Instances
- Bastion Host - Public Subnet - Public IP Enabled
- Private VM - Private Subnet - Public IP Disabled

6. Security Group Configuration
Bastion:
- Allow SSH from My IP

Private VM:
- Allow SSH only from Bastion Security Group

# Connection Process
1. SSH into Bastion Host
2. Copy private key to Bastion
3. SSH from Bastion to Private VM

Command: ssh -i private-key.pem ubuntu@PRIVATE_IP

# Verification
- Private VM not accessible directly from Internet
- Access only via Bastion
- Tested SSH connectivity successfully

# Architecture Diagram
Internet - Bastion Host (Public Subnet)  - Private VM (Private Subnet)

# Conclusion
Successfully implemented secure hybrid architecture using controlled access and network isolation.