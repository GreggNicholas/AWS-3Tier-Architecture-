# Overview
This lab provides a comprehensive hands-on experience in building a three-tier web architecture using Amazon Web Services (AWS). Participants will learn to create and configure the necessary components for a scalable and available web application, including networking, security, application, and database layers.
# Learning Objectives
S3 Bucket Creation: Set up an S3 bucket for code storage.
IAM Role Creation: Create an IAM role for EC2 instances to access S3 and Systems Manager.

Networking Setup: Build a secure VPC with subnets, route tables, internet gateways, and NAT gateways.
Database Deployment: Provision an Aurora MySQL database with Multi-AZ support.
Application Deployment: Launch an EC2 instance for the application tier, configure the software stack, and test database connectivity.
Load Balancing and Autoscaling: Create an internal load balancer and configure autoscaling for high availability.

Architecture Components
Application Load Balancer: Distributes incoming traffic to EC2 instances running Nginx and React.js.
Web Tier: Hosts web servers that serve the frontend and redirect API calls.
Application Tier: Contains Node.js applications that interact with the database.
Database Layer: Utilizes Amazon Aurora MySQL for data storage.
# Prerequisites
An active AWS account.
A preferred IDE or text editor.
# Instructions
Setup
Create an S3 bucket in the AWS console.
Set up an IAM role with necessary permissions.
Networking and Security
Create a VPC with at least six subnets across two availability zones.
Configure route tables for public and private subnets.
Set up security groups to manage traffic flow between components.
Database Deployment
Create a subnet group for the database layer.
Provision an Aurora MySQL database instance.
Application Tier Instance Deployment
Launch an EC2 instance in a private subnet for the application tier.
Connect to the instance using Systems Manager Session Manager.
Install necessary software and deploy the application code from S3.
Internal Load Balancing and Autoscaling
Create an AMI from the app tier instance.
Set up an internal load balancer to distribute traffic among app instances.
Configure autoscaling policies to manage instance scaling based on demand.
# Conclusion
By completing this lab, participants will gain practical experience in deploying a robust three-tier architecture on AWS, enhancing their cloud operations skills and understanding of scalable web applications. This summary encapsulates key elements of the lab assignment, providing a clear guide for users to understand the objectives and steps involved in setting up a three-tier architecture on AWS.

Full Instructions: https://github.com/GreggNicholas/AWS-3Tier-Architecture-/blob/main/3TWebArchLab%20(1).pdf

![3TierArch](https://github.com/GreggNicholas/AWS-3Tier-Architecture-/blob/main/3Tierarch.png?raw=true)

