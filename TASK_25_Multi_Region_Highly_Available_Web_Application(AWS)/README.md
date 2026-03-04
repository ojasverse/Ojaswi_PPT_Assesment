# TASK 25 - Multi-Region Highly Available Web Application (AWS)

## Objective
To deploy a highly available and fault-tolerant web application using AWS services across multiple Availability Zones.

# Architecture Overview
This architecture ensures high availability by distributing resources across multiple Availability Zones.
Traffic Flow:
User - Application Load Balancer - Target Group - EC2 (Private Subnets) - S3

# Services Used
Amazon VPC
Amazon EC2
Application Load Balancer (ALB)
Auto Scaling Group
Amazon S3
Amazon CloudWatch
NAT Gateway
Internet Gateway

# Implementation Steps
Created Custom VPC (10.0.0.0/16)
Created 2 Public Subnets (Different AZs)
Created 2 Private Subnets (Different AZs)
Attached Internet Gateway to VPC
Created NAT Gateway for private subnet internet access
Launched EC2 instances in Private Subnets
Created Security Groups (ALB - EC2)
Created Application Load Balancer
Configured Target Group and registered EC2 instances
Created Auto Scaling Group (Min:2, Desired:2)
Created S3 bucket for static assets
Configured CloudWatch Alarm (CPU > 70%)

# Testing & Validation
Accessed application using ALB DNS
Stopped one EC2 instance to test high availability
Verified Auto Scaling behavior


# Screenshots Included -
VPC configuration
ALB configuration
Auto Scaling Group
CloudWatch Alarm
Application running proof