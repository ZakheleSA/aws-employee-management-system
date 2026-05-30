# AWS Employee Management System

## Project Overview

This project demonstrates the design and implementation of a highly available 3-tier web application on AWS.

The goal is to deepen my understanding of:

- AWS Networking
- Compute
- Storage
- Databases
- Security
- Monitoring

## Architecture Components

### Networking
- Custom VPC (10.0.0.0/16)
- Public Subnets
- Private Subnets
- Internet Gateway
- Route Tables

### Compute
- EC2 Instances
- Auto Scaling Group
- Application Load Balancer

### Database
- Amazon RDS MySQL

### Storage
- Amazon S3

### Monitoring
- Amazon CloudWatch
- Amazon SNS

## Project Progress

### Completed
- [x] Custom VPC
- [x] Public Subnets
- [x] Private Subnets
- [x] Internet Gateway
- [x] Public Route Table

### In Progress
- [ ] Security Groups
- [ ] EC2 Instances
- [ ] Load Balancer
- [ ] RDS Database
- [ ] S3 Storage
- [ ] Monitoring

## Lessons Learned

### IAM Troubleshooting

Issue:
IAM user could not create VPC resources despite AdministratorAccess.

Root Cause:
An explicit deny was inherited through a user group policy.

Resolution:
Removed the user from the restricted group and used direct AdministratorAccess permissions.

Key Lesson:
Explicit Deny always overrides Allow permissions.
