# Terraform AWS VPC Infrastructure

This project provisions a basic AWS VPC infrastructure using Terraform.

## Architecture

```text
                    AWS
                     |
                    VPC
               10.0.0.0/16
                /         \
               /           \
      Public Subnet     Private Subnet
       10.0.1.0/24       10.0.2.0/24
            |
     Internet Gateway
```

## Resources Created

* AWS VPC
* Public Subnet
* Private Subnet
* Internet Gateway
* Public Route Table
* Public Route Table Association

## Terraform Structure

```text
terraform-aws-vpc-infrastructure/
│
├── provider.tf
├── main.tf
├── variables.tf
├── outputs.tf
├── terraform.tfvars
├── .gitignore
└── README.md
```

## Prerequisites

* AWS account
* AWS CLI configured
* Terraform installed
* Appropriate AWS IAM permissions

## How to Use

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/terraform-aws-vpc-infrastructure.git
cd terraform-aws-vpc-infrastructure
```

### 2. Initialize Terraform

```bash
terraform init
```

### 3. Format the configuration

```bash
terraform fmt
```

### 4. Validate the configuration

```bash
terraform validate
```

### 5. Review the execution plan

```bash
terraform plan
```

### 6. Create the infrastructure

```bash
terraform apply
```

Type:

```text
yes
```

when prompted.

## Destroy Resources

To remove the infrastructure created by Terraform
