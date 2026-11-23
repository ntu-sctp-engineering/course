# Platform Engineering Course Outline

## Module 1 - Cloud Computing Foundations (2 weeks)

| Week | Unit | Lesson | Summary |
| ---- | ---- | ------ | ------- |
| 1 | 1.1 | Introduction to Cloud Computing | Explains why organisations move from on-premise to cloud, covering virtualisation, service and deployment models (IaaS, PaaS, SaaS), the shared responsibility model and AWS Regions and Availability Zones. |
| 1 | 1.2 | Linux Essentials | Builds working confidence on the Linux command line, covering the file system, permissions, users, package managers, processes and managing services with systemctl. |
| 1 | 1.3 | Networking Essentials | Covers the networking every cloud engineer needs: IP addressing and CIDR subnets, ports, TCP vs UDP, DNS, and the HTTP, TLS and SSH protocols, tested with cURL and dig. |
| 2 | 1.4 | Cloud Security and Identity | Introduces security basics through the CIA triad, encryption and hashing, then applies least privilege with AWS IAM users, groups, roles, policies and MFA. |
| 2 | 1.5 | Cloud Networking with VPC | Designs a VPC with public and private subnets, route tables, internet and NAT gateways, and controls traffic with security groups and NACLs. |
| 2 | 1.6 | Compute in the Cloud | Launches and connects to EC2 instances (AMIs, instance types, key pairs, user data and EBS) and deploys a web server into the VPC built in the previous lesson. |

## Module 2 - Cloud Architecture and IaC (4 weeks)

| Week | Unit | Lesson | Summary |
| ---- | ---- | ------ | ------- |
| 3 | 2.1 | Well-Architected Design and Resilience | Applies the six pillars of the AWS Well-Architected Framework and the basics of high availability and disaster recovery (multi-AZ design, availability targets, backups, RTO and RPO) through a group architecture review. |
| 3 | 2.2 | Infrastructure as Code with Terraform | Introduces Infrastructure as Code and the Terraform init, plan, apply and destroy workflow by rebuilding the Module 1 VPC and EC2 web server as code in a Git repository. |
| 3 | 2.3 | Terraform Variables, Outputs and State | Makes configurations reusable with variables, outputs, locals and data sources, and explains Terraform state, remote S3 backends and state locking for team work. |
| 4 | 2.4 | Terraform Modules | Packages infrastructure into reusable custom modules, uses community modules from the Terraform Registry, and applies tagging, formatting and validation conventions. |
| 4 | 2.5 | Load Balancing and Auto Scaling | Builds a highly available web tier in Terraform with an Application Load Balancer, target groups and health checks, an Auto Scaling group across AZs, and HTTPS through Route 53 and ACM. |
| 4 | 2.6 | IAM as Code | Puts the IAM basics from Module 1 into practice by writing least-privilege roles, policies and instance profiles in Terraform so workloads can reach AWS services without access keys. |
| 5 | 2.7 | Storage and Content Delivery | Compares S3, EBS and EFS, then uses Terraform to host a private S3 static site behind CloudFront with origin access control, versioning and lifecycle rules. |
| 5 | 2.8 | Managed Databases | Chooses between relational and NoSQL databases and provisions RDS (multi-AZ, read replicas, backups, encryption) and DynamoDB with Terraform. |
| 5 | 2.9 | Secrets and Configuration | Keeps credentials out of code by storing and rotating secrets in AWS Secrets Manager and Parameter Store, reading them at runtime, and handling sensitive values safely in Terraform. |
| 6 | 2.10 | Serverless Computing with Lambda | Introduces serverless and AWS Lambda (runtimes, triggers, permissions, packaging and VPC access), deploying functions with Terraform and triggering them from S3 events. |
| 6 | 2.11 | Serverless APIs and Event-Driven Architecture | Builds a REST API with API Gateway, Lambda and DynamoDB, then decouples services with SQS, SNS and EventBridge. |
| 6 | 2.12 | Cloud Cost and Architecture Review | Covers AWS pricing models, Cost Explorer, budgets and cost-aware tagging, then has teams review and cost a Terraform-built architecture against the Well-Architected pillars. |

## Module 3 - Agentic Workflows (4 weeks)

| Week | Unit | Lesson | Summary |
| ---- | ---- | ------ | ------- |
| 7 | 3.1 | | |
| 7 | 3.2 | | |
| 7 | 3.3 | | |
| 8 | 3.4 | | |
| 8 | 3.5 | | |
| 8 | 3.6 | | |
| 9 | 3.7 | | |
| 9 | 3.8 | | |
| 9 | 3.9 | | |
| 10 | 3.10 | | |
| 10 | 3.11 | | |
| 10 | 3.12 | | |

## Module 4 - DevSecOps and AI Ops (4 weeks)

| Week | Unit | Lesson | Summary |
| ---- | ---- | ------ | ------- |
| 11 | 4.1 | | |
| 11 | 4.2 | | |
| 11 | 4.3 | | |
| 12 | 4.4 | | |
| 12 | 4.5 | | |
| 12 | 4.6 | | |
| 13 | 4.7 | | |
| 13 | 4.8 | | |
| 13 | 4.9 | | |
| 14 | 4.10 | | |
| 14 | 4.11 | | |
| 14 | 4.12 | | |

## Module 5 - Orchestration and Platform Engineering (4 weeks)

| Week | Unit | Lesson | Summary |
| ---- | ---- | ------ | ------- |
| 15 | 5.1 | | |
| 15 | 5.2 | | |
| 15 | 5.3 | | |
| 16 | 5.4 | | |
| 16 | 5.5 | | |
| 16 | 5.6 | | |
| 17 | 5.7 | | |
| 17 | 5.8 | | |
| 17 | 5.9 | | |
| 18 | 5.10 | | |
| 18 | 5.11 | | |
| 18 | 5.12 | | |

## Module 6 - Site Reliability Engineering (4 weeks)

| Week | Unit | Lesson | Summary |
| ---- | ---- | ------ | ------- |
| 19 | 6.1 | | |
| 19 | 6.2 | | |
| 19 | 6.3 | | |
| 20 | 6.4 | | |
| 20 | 6.5 | | |
| 20 | 6.6 | | |
| 21 | 6.7 | | |
| 21 | 6.8 | | |
| 21 | 6.9 | | |
| 22 | 6.10 | | |
| 22 | 6.11 | | |
| 22 | 6.12 | | |

## Module 7 - Capstone (2 weeks)

| Week | Unit | Lesson | Summary |
| ---- | ---- | ------ | ------- |
| 23 | 7.1 | Project Consultation | |
| 23 | 7.2 | Project Consultation | |
| 23 | 7.3 | Guest Speaker | |
| 24 | 7.4 | Project Consultation | |
| 24 | 7.5 | Project Consultation | |
| 24 | 7.6 | Project Presentation | |
