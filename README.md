# aws-vpc-cloud-network-setup1
AWS VPC – Cloud Network Setup
# AWS VPC – Cloud Network Setup

## 1. Project Overview

This project demonstrates how to design and configure a Virtual Private Cloud (VPC) in Amazon Web Services (AWS).

The project includes creating a custom VPC, configuring public and private subnets, attaching an Internet Gateway, configuring route tables, and creating a security group.

## 2. Technologies Used

- Cloud Platform: AWS
- Service: Amazon VPC
- Region: Asia Pacific (Mumbai) – ap-south-1
- Networking: IPv4 CIDR
- Compute: Amazon EC2
- Operating System: Amazon Linux 2023
- Security: AWS Security Groups and Network ACLs

## 3. Network Architecture

| Component | Configuration |
|---|---|
| VPC | cloud-network-vpc |
| VPC CIDR | 10.0.0.0/16 |
| Public Subnet | cloud-public-subnet |
| Public CIDR | 10.0.1.0/24 |
| Private Subnet | cloud-private-subnet |
| Private CIDR | 10.0.2.0/24 |
| Internet Gateway | cloud-network-igw |
| Public Route Table | cloud-public-rt |
| Private Route Table | cloud-private-rt |
| Security Group | cloud-network-sg |

## 4. Project Implementation

### Step 1: Create VPC
Created a custom VPC using IPv4 CIDR block 10.0.0.0/16.

### Step 2: Create Subnets
Created two subnets:
- Public subnet: 10.0.1.0/24
- Private subnet: 10.0.2.0/24

### Step 3: Configure Internet Gateway
Created an Internet Gateway and attached it to the custom VPC.

### Step 4: Configure Route Tables
- Public route table: Configured default route 0.0.0.0/0 to the Internet Gateway.
- Private route table: Kept the local VPC route only.

### Step 5: Configure Security Group
Created a security group named cloud-network-sg and configured SSH access for administration.

### Step 6: Launch EC2 Instance
Launched an Amazon Linux 2023 EC2 instance in the public subnet and connected using EC2 Instance Connect.

### Step 7: Network Testing
Performed private IP, internet connectivity, and DNS resolution checks.

## 5. Screenshots

Project screenshots will be added to the screenshots folder.

## 6. Skills Demonstrated

- AWS VPC configuration
- Public and private subnet creation
- Internet Gateway configuration
- Route table management
- AWS Security Groups
- Network ACL basics
- EC2 deployment and connectivity troubleshooting
- Basic network connectivity testing

## 7. Project Outcome

Configured a custom AWS VPC with public and private subnets, an Internet Gateway, route tables, and a security group. Launched an EC2 instance in the public subnet and connected to it for network testing.

**Project Status:** Implementation completed. Connectivity test results should be documented with screenshots.
