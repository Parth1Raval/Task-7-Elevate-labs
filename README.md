# Task-7-Elevate-labs

# AWS Auto Scaling and Load Balancer Setup for Web Application

## Overview  
This project demonstrates how to build a scalable and high-availability web application infrastructure on AWS using core networking and compute services. By leveraging EC2 instances, an Application Load Balancer (ALB), and Auto Scaling groups, it showcases automation in handling traffic spikes, fault tolerance, and cost optimization.

## What It Does  
- Launches multiple EC2 instances running Apache HTTP Server with a basic HTML web page.  
- Distributes incoming web traffic evenly across these instances using an ALB for improved availability.  
- Automatically adjusts the number of running instances based on CPU load to handle changes in traffic smoothly without manual intervention.

## Key Components  
- **Amazon VPC & Subnets:** Isolated virtual network with multiple subnets across availability zones for redundancy.  
- **Launch Template:** Defines the EC2 instance configuration including OS image, specs, and web server setup.  
- **Auto Scaling Group:** Dynamically manages instance count between 1 and 4 based on predetermined CPU thresholds.  
- **Application Load Balancer:** Routes HTTP traffic to healthy EC2 instances, ensuring availability and seamless user experience.

## How to Use  
1. Deploy the launch template configured with Amazon Linux 2023 and Apache HTTP Server setup.  
2. Set up an Auto Scaling group using the launch template, selecting multiple subnets to enable multi-AZ deployment.  
3. Attach the Auto Scaling group to the Application Load Balancer target group for traffic distribution.  
4. Access the Load Balancer’s public URL to see the live web page served from your scalable backend.  
5. Optionally, simulate traffic to see Auto Scaling in action and monitor instance scaling events.

## Benefits Highlighted  
- High availability across multiple zones  
- Automatic scaling for cost optimization and performance  
- Easy traffic management through built-in load balancing


This setup serves as a foundational example for cloud scalability and fault-tolerance concepts in AWS, ideal for beginners learning modern cloud infrastructure principles.

