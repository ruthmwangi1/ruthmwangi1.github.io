---
title: "CloudFormation VPC + EC2 Setup"
layout: single
permalink: projects/vpc-ec2-setup/
---

## Infrastructure as Code with AWS CloudFormation

**Project Type:** Infrastructure as Code  
**Tools & Services:** AWS CloudFormation, VPC, Subnet, Security Group, EC2, Internet Gateway  
**Category:** Automation & Cloud Architecture


### Project Overview
This project demonstrates how to provision and manage AWS infrastructure using **Infrastructure as Code (IaC)** with **AWS CloudFormation**.
Instead of manually creating resources through the AWS Console, the entire environment is defined using a declarative YAML template, making deployment **repeatable, automated, and error-free**.


### Objectives
- Automate provisioning of AWS resources  
- Ensure consistent, reproducible infrastructure  
- Reduce human error in setup  
- Apply best practices for scalable and secure cloud architecture  

### Architecture & Resources Deployed
The CloudFormation template provisions:

- A **Virtual Private Cloud (VPC)**  
- A **Private Subnet**  
- An **Internet Gateway** attached to the VPC  
- A **Security Group** allowing SSH access  
- An **EC2 Instance** launched in the private subnet  
- Dynamic **Availability Zone selection** using `!GetAZs` and `!Select`  
- Parameterized **AMI ID** pulled from SSM for the latest Amazon Linux 2023 image  


### Key Concepts Demonstrated
- **Infrastructure as Code (IaC)**  
- **Automation & Reproducibility**  
- **Cloud Networking & Security**  
- **Best practices for parameterization and region-agnostic deployment**  


### Outcome
- Successfully deployed a fully functional AWS environment with a single template  
- Infrastructure can be **recreated or updated in minutes**  
- Gained hands-on experience in **VPC setup, EC2 provisioning, security groups, and automation**  


### Project Links 
- **CloudFormation Template:** [vpc-ec2-setup.yaml](https://github.com/Ruthie-tech/ruthmwangi.github.io/blob/master/templates/cloudformation/vpc-ec2-setup.yaml)
- **Template Instructions:** [README.md](https://github.com/Ruthie-tech/ruthmwangi.github.io/blob/master/templates/cloudformation/README.md)
