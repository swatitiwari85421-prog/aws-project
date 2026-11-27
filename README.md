# AWS Load Balancer and Auto Scaling Project

## Project Overview

This project demonstrates the deployment of a web server infrastructure on Amazon Web Services (AWS) using EC2 instances, an Application Load Balancer, Target Groups, and Auto Scaling.

The main objective is to distribute incoming web traffic across multiple EC2 instances and improve application availability and scalability.

## AWS Services Used

- **Amazon VPC:** Created a custom Virtual Private Cloud.
- **Subnets:** Configured subnets in different Availability Zones.
- **Amazon EC2:** Created virtual machines to host the website.
- **Amazon Machine Image (AMI):** Created an image of the configured web server.
- **Launch Template:** Configured instance launch settings.
- **Target Group:** Configured HTTP traffic routing on port 80.
- **Application Load Balancer:** Distributed incoming traffic across registered EC2 instances.
- **Auto Scaling Group:** Configured automatic instance management.

## Project Configuration

| Resource | Configuration |
|---|---|
| Region | US East (Ohio) |
| VPC | my-vpc-01 |
| Load Balancer | Webloadbalancer |
| Target Group | Web-Tg |
| Launch Template | Mytemplate |
| AMI | IMG1 |
| Auto Scaling Group | mysgn |
| Instance Type | t3.micro |
| Protocol | HTTP |
| Port | 80 |
| Desired Capacity | 2 |
| Minimum Capacity | 1 |
| Maximum Capacity | 2 |

## Architecture

The project follows this architecture:

Internet  
↓  
Application Load Balancer  
↓  
Target Group  
↓  
EC2 Web Server Instances

Auto Scaling Group manages the EC2 instances and maintains the desired capacity.

## Implementation Steps

1. Created a custom VPC.
2. Created subnets in different Availability Zones.
3. Launched EC2 instances.
4. Installed and configured the Apache web server.
5. Created an AMI from the configured web server.
6. Created a Launch Template using the AMI.
7. Created a Target Group with HTTP protocol on port 80.
8. Created an Application Load Balancer.
9. Attached the Target Group to the Load Balancer.
10. Created an Auto Scaling Group using the Launch Template.
11. Configured desired, minimum, and maximum instance capacity.
12. Integrated the Auto Scaling Group with the existing Target Group.

## Key Features

- Traffic distribution using Application Load Balancer.
- EC2 instance management using Auto Scaling.
- Custom VPC and subnet configuration.
- AMI-based instance deployment.
- Health checks for monitoring instance availability.

## Screenshots

AWS Console screenshots are available in the `screenshots` folder.

## Learning Outcomes

Through this project, I learned how to:

- Configure networking using Amazon VPC.
- Launch and manage EC2 instances.
- Create and use AMIs and Launch Templates.
- Configure Application Load Balancers.
- Create and manage Target Groups.
- Configure Auto Scaling Groups.
- Understand load balancing and scalability in AWS.

## Author

**Swati Tiwari,kirti,sneha,smriti,kavita,ritika.palak,niketa**

B.Tech Computer Science

## Technologies

- Amazon Web Services (AWS)
- Amazon EC2
- Application Load Balancer
- Auto Scaling
- Apache Web Server
- HTML