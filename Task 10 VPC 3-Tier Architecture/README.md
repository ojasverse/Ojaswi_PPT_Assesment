# Task 10: VPC 3-Tier Architecture

## Objective
To design and implement a secure 3-tier architecture (Web, App, Database) inside a custom VPC.

## Services Used
- Amazon VPC
- EC2
- Internet Gateway
- NAT Gateway
- Route Tables
- Security Groups
- NACL

## Architecture Overview
- Public Subnet → Web Tier (Accessible from Internet)
- Private Subnet 1 → Application Tier
- Private Subnet 2 → Database Tier
- NAT Gateway for private subnet internet access
- Internet Gateway for public subnet

## Implementation Steps
1. Created custom VPC with CIDR block.
2. Created 2 public and 2 private subnets.
3. Attached Internet Gateway.
4. Created NAT Gateway in public subnet.
5. Configured Route Tables.
6. Launched EC2 instances in respective subnets.
7. Configured Security Groups.

## Proof
- Screenshots

## Outcome
Successfully implemented secure and scalable 3-tier architecture.
