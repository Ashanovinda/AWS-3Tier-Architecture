# Highly Available & Secure 3-Tier Web Architecture on AWS

## Project Overview
Designed and deployed a highly available, scalable, and secure 3-tier architecture on AWS to host a web application (Crypto Trading Platform). The infrastructure ensures high availability through Auto Scaling and Multi-AZ database deployments while maintaining strict security via private subnets and Security Groups.

## Architecture Diagram
![Architecture Diagram](AWS%203-Tier%20Architecture.drawio.png)

## Core Technologies & AWS Services Used:
* **Networking:** Custom VPC, Internet Gateway, NAT Gateway, Public & Private Subnets.
* **Compute:** EC2 (Amazon Linux 2023), Auto Scaling Group, Application Load Balancer (ALB).
* **Database:** Amazon RDS (MySQL) configured with Multi-AZ for failover.
* **Security:** Strict Security Group rules allowing minimum required access.

## Key Features:
* **High Availability:** Web servers are spread across 2 Availability Zones and managed by an Auto Scaling Group to handle traffic spikes.
* **Enhanced Security:** Compute resources and databases are isolated in private subnets, completely hidden from direct internet access.
* **Outbound Internet Access:** A NAT Gateway is used to allow private instances to securely download software updates.
* **Database Reliability:** Multi-AZ RDS ensures automatic failover to a standby database in case of an infrastructure failure.
