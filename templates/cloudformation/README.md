# CloudFormation VPC + EC2 Setup

This template provisions a basic AWS environment using **Infrastructure as Code (IaC)**:

## Resources created

- VPC with CIDR 10.0.0.0/16
- Private Subnet with CIDR 10.0.1.0/24
- Internet Gateway
- Security Group allowing SSH
- EC2 instance using latest Amazon Linux 2023 AMI

## How to deploy

1. Open AWS CloudFormation console
2. Click "Create stack"
3. Upload `vpc-ec2-setup.yaml`
4. Provide any parameters if needed (e.g., AMI ID)
5. Deploy and wait for completion

## Notes

- Uses `!GetAZs` and `!Select` to dynamically select Availability Zone
- Parameterized AMI ID from SSM for up-to-date image
