# Platform Engineering Course Outline

## Module 1 - Cloud Computing Foundations (2 weeks)

### Week 1

Sets up the foundations: why organisations move to the cloud, working on the Linux command line, and the networking concepts (IP, CIDR, DNS, HTTP, TLS, SSH) every cloud engineer relies on.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 1.1 | Introduction to Cloud Computing | Explains why organisations move from on-premise to cloud, covering virtualisation, service and deployment models (IaaS, PaaS, SaaS), the shared responsibility model and AWS Regions and Availability Zones. |
| 1.2 | Linux Essentials | Builds working confidence on the Linux command line, covering the file system, permissions, users, package managers, processes and managing services with systemctl. |
| 1.3 | Networking Essentials | Covers the networking every cloud engineer needs: IP addressing and CIDR subnets, ports, TCP vs UDP, DNS, and the HTTP, TLS and SSH protocols, tested with cURL and dig. |

### Week 2

Moves into AWS: securing accounts with IAM and least privilege, designing a VPC with public and private subnets, and launching an EC2 web server into it.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 1.4 | Cloud Security and Identity | Introduces security basics through the CIA triad, encryption and hashing, then applies least privilege with AWS IAM users, groups, roles, policies and MFA. |
| 1.5 | Cloud Networking with VPC | Designs a VPC with public and private subnets, route tables, internet and NAT gateways, and controls traffic with security groups and NACLs. |
| 1.6 | Compute in the Cloud | Launches and connects to EC2 instances (AMIs, instance types, key pairs, user data and EBS) and deploys a web server into the VPC built in the previous lesson. |

## Module 2 - Cloud Architecture and IaC (4 weeks)

### Week 3

Starts designing for resilience with the Well-Architected Framework, then introduces Terraform and remote state so all later infrastructure is built as code.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 2.1 | Well-Architected Design and Resilience | Applies the six pillars of the AWS Well-Architected Framework and the basics of high availability and disaster recovery (multi-AZ design, availability targets, backups, RTO and RPO) through a group architecture review. |
| 2.2 | Infrastructure as Code with Terraform | Introduces Infrastructure as Code and the Terraform init, plan, apply and destroy workflow by rebuilding the Module 1 VPC and EC2 web server as code in a Git repository. |
| 2.3 | Terraform Variables, Outputs and State | Makes configurations reusable with variables, outputs, locals and data sources, and explains Terraform state, remote S3 backends and state locking for team work. |

### Week 4

Grows the Terraform skills with reusable modules, then builds a highly available web tier with a load balancer and auto scaling, and writes IAM roles and policies as code.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 2.4 | Terraform Modules | Packages infrastructure into reusable custom modules, uses community modules from the Terraform Registry, and applies tagging, formatting and validation conventions. |
| 2.5 | Load Balancing and Auto Scaling | Builds a highly available web tier in Terraform with an Application Load Balancer, target groups and health checks, an Auto Scaling group across AZs, and HTTPS through Route 53 and ACM. |
| 2.6 | IAM as Code | Puts the IAM basics from Module 1 into practice by writing least-privilege roles, policies and instance profiles in Terraform so workloads can reach AWS services without access keys. |

### Week 5

Adds the data layer: S3, EBS and EFS storage with CloudFront, managed RDS and DynamoDB databases, and keeping secrets out of code with Secrets Manager and Parameter Store.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 2.7 | Storage and Content Delivery | Compares S3, EBS and EFS, then uses Terraform to host a private S3 static site behind CloudFront with origin access control, versioning and lifecycle rules. |
| 2.8 | Managed Databases | Chooses between relational and NoSQL databases and provisions RDS (multi-AZ, read replicas, backups, encryption) and DynamoDB with Terraform. |
| 2.9 | Secrets and Configuration | Keeps credentials out of code by storing and rotating secrets in AWS Secrets Manager and Parameter Store, reading them at runtime, and handling sensitive values safely in Terraform. |

### Week 6

Goes serverless with Lambda, API Gateway and event-driven services (SQS, SNS, EventBridge), and closes the module with a cost and architecture review.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 2.10 | Serverless Computing with Lambda | Introduces serverless and AWS Lambda (runtimes, triggers, permissions, packaging and VPC access), deploying functions with Terraform and triggering them from S3 events. |
| 2.11 | Serverless APIs and Event-Driven Architecture | Builds a REST API with API Gateway, Lambda and DynamoDB, then decouples services with SQS, SNS and EventBridge. |
| 2.12 | Cloud Cost and Architecture Review | Covers AWS pricing models, Cost Explorer, budgets and cost-aware tagging, then has teams review and cost a Terraform-built architecture against the Well-Architected pillars. |

## Module 3 - Agentic Workflows (4 weeks)

### Week 7

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 3.1 | | |
| 3.2 | | |
| 3.3 | | |

### Week 8

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 3.4 | | |
| 3.5 | | |
| 3.6 | | |

### Week 9

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 3.7 | | |
| 3.8 | | |
| 3.9 | | |

### Week 10

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 3.10 | | |
| 3.11 | | |
| 3.12 | | |

## Module 4 - DevSecOps and AI Ops (4 weeks)

### Week 11

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 4.1 | | |
| 4.2 | | |
| 4.3 | | |

### Week 12

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 4.4 | | |
| 4.5 | | |
| 4.6 | | |

### Week 13

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 4.7 | | |
| 4.8 | | |
| 4.9 | | |

### Week 14

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 4.10 | | |
| 4.11 | | |
| 4.12 | | |

## Module 5 - Orchestration and Platform Engineering (4 weeks)

### Week 15

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 5.1 | | |
| 5.2 | | |
| 5.3 | | |

### Week 16

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 5.4 | | |
| 5.5 | | |
| 5.6 | | |

### Week 17

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 5.7 | | |
| 5.8 | | |
| 5.9 | | |

### Week 18

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 5.10 | | |
| 5.11 | | |
| 5.12 | | |

## Module 6 - Site Reliability Engineering (4 weeks)

### Week 19

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 6.1 | | |
| 6.2 | | |
| 6.3 | | |

### Week 20

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 6.4 | | |
| 6.5 | | |
| 6.6 | | |

### Week 21

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 6.7 | | |
| 6.8 | | |
| 6.9 | | |

### Week 22

To be designed.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 6.10 | | |
| 6.11 | | |
| 6.12 | | |

## Module 7 - Capstone (2 weeks)

### Week 23

Teams build their capstone projects with instructor consultations, and hear from an industry guest speaker.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 7.1 | Project Consultation | |
| 7.2 | Project Consultation | |
| 7.3 | Guest Speaker | |

### Week 24

Teams finish their capstone projects with final consultations, then present them.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 7.4 | Project Consultation | |
| 7.5 | Project Consultation | |
| 7.6 | Project Presentation | |
