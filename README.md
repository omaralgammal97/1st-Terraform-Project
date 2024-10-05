# Terraform AWS Infrastructure Project

This Terraform project provisions a complete AWS infrastructure, including VPC, subnets, EC2 instances, load balancers, S3 bucket for state management, and DynamoDB for state locking.

## Prerequisites

- [Terraform](https://www.terraform.io/downloads.html) installed on your machine.
- An AWS account with IAM permissions to create the resources defined in this project.
- AWS CLI configured with the appropriate access credentials.

## Project Structure

```plaintext
terraform-project/
├── main.tf             # Main Terraform configuration
├── variables.tf        # Variable definitions
├── outputs.tf          # Output values from Terraform
├── modules/            # Contains reusable modules
│   ├── ec2/            # EC2 module for provisioning instances
│   ├── loadbalancer/   # Load balancer module
│   ├── subnet/         # Subnet module
│   └── vpc/            # VPC module
└── ...
