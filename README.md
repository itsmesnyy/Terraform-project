
# 🚀 AWS Infrastructure Automation using Terraform

This project provisions a **secure, scalable, and production-ready AWS infrastructure** using Terraform. It supports multi-tier application deployment by automating services like **Elastic Beanstalk**, **EC2**, **RDS (MySQL)**, **ElastiCache**, **ActiveMQ**, and a **Bastion Host**—all written in modular, reusable code for consistent development and production environments.

---

## 📌 Key Features

- ✅ Infrastructure as Code (IaC) using Terraform
- 🔐 Secure architecture with Bastion Host, private subnets, and strict security groups
- 🧱 Modular Terraform configuration for VPC, compute, database, cache, messaging, and application layers
- 📦 Fully automated provisioning of:
  - VPC, subnets, route tables, NAT gateway, Internet gateway
  - EC2 instances with remote provisioning via `remote-exec`
  - Elastic Beanstalk environment with Tomcat 10 on Corretto 21
  - RDS (MySQL) as the backend database
  - ElastiCache (Redis) for caching
  - ActiveMQ for asynchronous messaging
- 📉 Reduced infrastructure provisioning time by 3×
- 🛠️ Improved deployment reliability and reproducibility across environments

---

## 🧰 Tech Stack

| Tool        | Purpose                                  |
|-------------|-------------------------------------------|
| Terraform   | Infrastructure automation (IaC)           |
| AWS         | Cloud infrastructure                      |
| EC2         | Compute layer                             |
| RDS         | Managed MySQL database                    |
| ElastiCache | Redis-based caching layer                 |
| ActiveMQ    | Messaging queue broker                    |
| Elastic Beanstalk | Application orchestration           |


## ⚙️ Getting Started

### ✅ Prerequisites

- Terraform v1.3+
- AWS CLI installed and configured
- AWS credentials set via `aws configure`
- SSH key pair created in your AWS region

### 🔧 Setup Steps

1. Clone the Repository

2. Initialize Terraform
   terraform init

3. Validate the configuration
   terraform validate

4. Preview the execution plan
   terraform plan

5. Apply the configuration
   terraform apply

6. (Optional) Destroy the infrastructure
   terraform destroy



## 📤 Outputs

- Bastion Host Public IP
- Elastic Beanstalk Application URL
- RDS Endpoint
- ElastiCache Endpoint
- ActiveMQ Endpoint (if applicable)

---

## 🧠 Design Considerations

- Built for multi-tier architecture
- Network segmentation using public and private subnets
- Auto-provisioned compute, database, and messaging layers
- Modularized code for reusability
- Blue/green deployment via Elastic Beanstalk
- All services in a single AWS region

---

## 👤 Author

Santhi Yanamala  
Email: santhiyanamala6@gmail.com  
LinkedIn: https://www.linkedin.com/in/santhi-yanamala
