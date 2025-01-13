# Portfolio Website

Hello! Hemanth Kumar s Here!   

This is the Portfolio Website and below is simple webserver
![image](https://github.com/user-attachments/assets/a7a045c0-3d82-4c9d-9e35-88e12c6c5df6)



PHP Webserver Hosted on AWS with Elastic Load Balancer (ELB) 

This project sets up a scalable, secure, and highly available PHP webserver hosted on AWS EC2 instances. The infrastructure uses Elastic Load Balancer (ELB) to distribute traffic and follows security best practices to ensure data and network safety and auto-scale to scale as required

Architecture Overview

The architecture includes:

VPC: A Virtual Private Cloud divided into public and private subnets across multiple availability zones for high availability.

Public Subnets: Used for NAT gateways to enable internet access for instances in private subnets.

Private Subnets: Host EC2 instances that run the PHP webserver. Instances are managed via an Auto Scaling Group to ensure scalability.

Application Load Balancer (ALB): Distributes incoming traffic across the EC2 instances in private subnets.

S3 Gateway: Ensures only private EC2 instances can securely read/write data to S3 buckets.

Security Groups: Restrict access to resources based on specific inbound and outbound traffic rules.


