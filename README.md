# Terraform AWS Infrastructure

## 📌 Project Overview

This project demonstrates how to provision and manage AWS infrastructure using **Terraform Infrastructure as Code (IaC)**.

The project creates an AWS EC2 instance using reusable Terraform configuration with input variables and output values.

## 🏗️ Architecture

```text
Terraform
    │
    ▼
AWS Provider
    │
    ▼
EC2 Instance
    │
    ├── Instance ID
    ├── Public IP
    └── Public DNS
```

## 🛠️ Technologies Used

* Terraform
* AWS
* Amazon EC2
* Infrastructure as Code
* Git
* GitHub

## 📂 Project Structure

```text
terraform-aws-infrastructure/
│
├── main.tf
├── variables.tf
└── outputs.tf
```

### `main.tf`

Contains the AWS provider configuration and EC2 instance resource.

### `variables.tf`

Defines configurable Terraform variables such as:

* AWS region
* AMI ID
* EC2 instance type

### `outputs.tf`

Displays information about the created EC2 instance:

* Instance ID
* Public IP address
* Public DNS

## 🚀 How to Use

### 1. Install Terraform

Make sure Terraform is installed and configured on your system.

### 2. Configure AWS Credentials

Configure your AWS credentials using the AWS CLI or another supported authentication method.

### 3. Clone the Repository

```bash
git clone https://github.com/Seran2304/terraform-aws-infrastructure.git
cd terraform-aws-infrastructure
```

### 4. Initialize Terraform

```bash
terraform init
```

### 5. Create a Terraform Variables File

Create a local `terraform.tfvars` file:

```hcl
aws_region    = "ap-south-1"
ami_id        = "YOUR_AMI_ID"
instance_type = "t2.micro"
```

Replace `YOUR_AMI_ID` with a valid AMI ID for your selected AWS region.

### 6. Validate the Configuration

```bash
terraform validate
```

### 7. Review the Execution Plan

```bash
terraform plan
```

### 8. Apply the Infrastructure

```bash
terraform apply
```

Type `yes` when prompted.

### 9. Destroy the Infrastructure

When the resources are no longer required:

```bash
terraform destroy
```

## 🔐 Security Note

Do not commit AWS access keys, secret keys, passwords, or other sensitive information to GitHub.

The `terraform.tfvars` file should remain local if it contains environment-specific or sensitive values.

## 🎯 Learning Outcomes

Through this project, I practiced:

* Infrastructure as Code using Terraform
* AWS provider configuration
* EC2 provisioning
* Terraform variables
* Terraform outputs
* Terraform lifecycle commands
* Git and GitHub repository management

## 👨‍💻 Author

**Seran Rajamani**

GitHub: https://github.com/Seran2304
