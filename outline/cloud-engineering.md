# Cloud Engineering Course Outline

## Module 1 - IT Infrastructure Essentials (6 weeks)

| Week | Unit | Lesson | Summary |
| ---- | ---- | ------ | ------- |
| 1 | 1.1 | Introduction to IT Infrastructure | Compares on-premise and cloud infrastructure, covering virtualisation, cloud deployment and service models (IaaS, PaaS, SaaS), and the cost and scalability trade-offs. |
| 1 | 1.2 | Networking Essentials | Introduces networking basics such as IP and MAC addresses, routers, switches and DNS, then maps them to AWS VPC and Route 53. |
| 2 | 1.3 | Network Communications Protocol | Covers the OSI and TCP/IP models, TCP vs UDP, common application protocols like HTTP, SSH and TLS, and calling a REST API with Postman or cURL. |
| 2 | 1.4 | Basic Security | Surveys IT security across IAM, network, application, data and cloud security, using the CIA triad, hashing and an OpenSSL encryption activity. |
| 2 | CO | Coaching 1 | Walks learners through installing and verifying the course toolchain (WSL or macOS terminal, VS Code, Git, Docker, Terraform, Node, Python, kubectl, Helm, AWS CLI). |
| 3 | 1.5 | Servers Administration I | Compares Windows and Linux servers (shells, package managers, services, file permissions) and has learners launch and connect to both on EC2. |
| 3 | 1.6 | Servers Administration II | Explains programs, processes, threads, CPU, memory and storage, and has learners run an Apache web server on EC2 with systemctl. |
| 3 | CO | Coaching 2 | Has learners build a simple Python Flask app, push it to GitHub and run it on EC2 behind an httpd reverse proxy. |
| 4 | 1.7 | Network Security | Walks through securing traffic from the internet to EC2 with VPC subnets, gateways, VPC endpoints, NACLs and security groups. |
| 4 | 1.8 | High Availability & Disaster Recovery | Covers RAID levels, availability "nines" and downtime maths, AWS Regions and AZs, and HA practices such as backups, failover and RTO/RPO planning. |
| 4 | CO | Coaching 3 | Hosts the Flask app in an EC2 Auto Scaling group from a launch template, then load-tests scale-out and simulates self-healing. |
| 5 | 1.9 | Load Balancing | Explains load-balancing types and algorithms, Layer 4 vs Layer 7 balancing, and AWS ALB and NLB with target groups, listeners and health checks. |
| 5 | 1.10 | Database I | Introduces relational databases, keys, ACID and SQL command types, with AWS RDS and a self-hosted MariaDB on EC2 activity. |
| 5 | CO | Coaching 4 | Sets up host-based routing on an ALB for two apps with Route 53 aliases, then adds ACM certificates and an HTTPS listener. |
| 6 | 1.11 | Database II | Compares SQL and NoSQL, tours document, key-value, columnar and graph databases and their AWS services, with a self-hosted MongoDB activity. |
| 6 | 1.12 | Cloud Migration | Covers cloud migration benefits and challenges, the migration lifecycle, the 6 Rs and AWS migration services, with a group migration-plan case study. |
| 6 | CO | Coaching 5 | Builds a three-tier VPC in the console with public, private and database subnets, route tables, an internet gateway and a NAT gateway. |

## Module 2 - Cloud Technologies Essentials and Architectural Design (10 weeks)

| Week | Unit | Lesson | Summary |
| ---- | ---- | ------ | ------- |
| 1 | 2.1 | Principles in Cloud Arch. Design | Reviews core cloud characteristics and the six pillars of the AWS Well-Architected Framework, ending with a group architecture review against them. |
| 1 | 2.2 | Infrastructure as Code 1 | Introduces Infrastructure as Code and Terraform's write, plan, apply workflow, with learners declaring their first provider and resource blocks. |
| 1 | CO | Coaching 6 | Provisions an EC2 instance and SSH security group with Terraform (init, plan, apply, destroy) and commits the code to GitHub. |
| 2 | 2.3 | Infrastructure as Code 2 | Covers Terraform block types (data, variable, output, locals, terraform) and remote S3 backends, with an assignment to output an EC2 instance's public IP and DNS. |
| 2 | 2.4 | Infrastructure as Code 3 | Teaches Terraform modules (community and custom), conditional expressions and functions, plus tagging and pre-commit hook best practices. |
| 2 | CO | Coaching 7 | Builds a reusable Terraform web-app module with configurable instance count and a public/private subnet toggle, then adds ALB path-based routing to it. |
| 3 | 2.5 | Database as a Service | Explores managed databases on AWS, covering DynamoDB and RDS/Aurora features like replication, backups and encryption, with an assignment to build a DynamoDB table in Terraform. |
| 3 | 2.6 | Identity Access Management | Explains authentication vs authorisation and AWS IAM users, groups, roles and policy types, with an activity giving an EC2 instance access to DynamoDB. |
| 3 | CO | Coaching 8 | Creates IAM roles, policies and instance profiles in Terraform, then gives an EC2 instance access to DynamoDB (optionally connecting to RDS). |
| 4 | 2.7 | Storage | Compares AWS S3, EBS and EFS storage, with activities on S3 versioning and lifecycle rules, mounting EBS volumes and sharing EFS across instances. |
| 4 | 2.8 | Deployment as a Service | Surveys AWS deployment services (Lightsail, Elastic Beanstalk, CodeDeploy, CloudFormation, ECS/EKS) and deploys an application with Elastic Beanstalk. |
| 4 | CO | Coaching 9 | Hosts a static website on a public S3 bucket with a Route 53 alias, then recreates it in Terraform. |
| 5 | 2.9 | Security | Maps AWS security services to prevention, detection and governance (WAF, GuardDuty, Inspector, Config, Security Hub), with a WAF rules activity on an ALB. |
| 5 | 2.10 | Networking 1 | Explains CDNs, CloudFront and Global Accelerator, with an activity serving an S3 static site through CloudFront on a custom HTTPS domain. |
| 5 | CO | Coaching 10 | Uses Terraform to serve a private S3 static site through CloudFront with OAC, adding ACM, Route 53 and WAF as a challenge. |
| 6 | 2.11 | Networking 2 | Covers VPC connectivity options (NAT, peering, Transit Gateway, VPN, Direct Connect) and VPC endpoints, with a VPC peering activity. |
| 6 | 2.12 | Function as a Service | Introduces serverless and AWS Lambda configuration, invocation, permissions and monitoring, with an activity triggering Lambda from S3 uploads. |
| 6 | CO | Coaching 11 | Deploys a Python Lambda inside a VPC with its own security group and a pymysql package so it can query a MySQL RDS database. |
| 7 | 2.13 | Serverless Architecture 1 | Introduces microservices and serverless architecture with Amazon API Gateway, and builds a REST API backed by Lambda and DynamoDB. |
| 7 | 2.14 | Serverless Architecture 2 | Covers event-driven messaging with SQS, SNS and EventBridge, with activities wiring each to Lambda. |
| 7 | CO | Coaching 12 | Fixes a starter Terraform repo to build a serverless Movies API from DynamoDB, Lambda and API Gateway, then adds logging and a custom domain. |
| 8 | 2.15 | Secret Management | Explains secret management practices and anti-patterns, with activities storing and retrieving secrets in AWS Secrets Manager and Parameter Store. |
| 8 | 2.16 | Cost and Monitoring | Covers AWS cost tools (Cost Explorer, Reserved Instances, Savings Plans, Trusted Advisor) and observability with CloudWatch logs, metrics and alarms and CloudTrail. |
| 8 | CO | Coaching 13 | Practises the Git workflow (init, add, commit, push to GitHub), branching, merging and pull requests, with a reading on branching strategies. |
| 9 | CO | Coaching 14 | Teams collaborate on one repo to resolve divergence and merge conflicts, then use GitHub rulesets to block force pushes and require reviewed PRs. |
| 10 | CO | Coaching 15 | |

## Module 3 - DevSecOps Essentials and System Monitoring Strategies (8 weeks)

| Week | Unit | Lesson | Summary |
| ---- | ---- | ------ | ------- |
| 1 | 3.1 | Introduction to DevSecOps | Traces the path from SDLC and Agile to DevOps and DevSecOps, then introduces GitHub Actions with a basic workflow and an OIDC-based Terraform deploy to AWS. |
| 1 | 3.2 | DevSecOps and Workflow | Covers pull requests, branch protection rulesets, Terraform CI checks, GitHub Environments and reusable workflows. |
| 1 | CO | Coaching 16 | Groups build a serverless URL shortener (API Gateway, Lambda, DynamoDB, WAF, X-Ray) in Terraform, delivered through PR-protected CI/CD. |
| 2 | 3.3 | Introduction to Container | Introduces containers and Docker (Dockerfiles, images, registries), with activities building a Flask image and pushing it to Docker Hub. |
| 2 | 3.4 | Container Orchestration with ECS Part 1 | Introduces Amazon ECR and ECS (clusters, task definitions, services, Fargate), with activities pushing an image to ECR and running it on ECS. |
| 2 | CO | Coaching 17 | Provisions ECR and ECS Fargate with Terraform, then uses GitHub Actions to build the sample app image and deploy it to ECS. |
| 3 | 3.5 | Container Orchestration with ECS Part 2 | Covers ECS environment variables, injecting Secrets Manager and Parameter Store values into task definitions, and X-Ray sidecar containers. |
| 3 | 3.6 | Package Vulnerability Scanning | Explains package vulnerability scanning techniques and best practices, with hands-on Snyk scans of code, Terraform, container images and dependencies. |
| 3 | CO | Coaching 18 | Pairs deploy two Flask services (S3 upload and SQS messaging) to one ECS cluster, splitting IaC and app CI/CD across protected repos. |
| 4 | 3.7 | Container Orchestration with EKS Part 1 | Introduces Kubernetes architecture, pods, ReplicaSets, deployments, namespaces and service accounts, then deploys resources to a shared Amazon EKS cluster. |
| 4 | 3.8 | Container Orchestration with EKS Part 2 | Covers Kubernetes Services (ClusterIP, NodePort, LoadBalancer), Ingress controllers, and ConfigMaps and Secrets with secret-management best practices. |
| 4 | CO | Coaching 19 | Deploys an echo app on a shared EKS cluster and exposes it via an NGINX Ingress with ExternalDNS records and a Let's Encrypt TLS cert from cert-manager. |
| 5 | 3.9 | Monitoring for Container | Covers Kubernetes monitoring with Prometheus (installed via Helm), ServiceMonitors and PromQL, plus Alertmanager and Grafana. |
| 5 | 3.10 | Logging for Container | Explains centralised logging challenges in Kubernetes and sets up Grafana Loki with Promtail to collect and query container logs in Grafana. |
| 5 | CO | Coaching 20 | Installs Prometheus with Alertmanager via Helm on EKS, writes PromQL for node CPU and memory use, and routes an alert rule to a webhook. |
| 6 | 3.11 | Package Manager for Container 1 | Introduces package managers and Helm charts, releases and repositories, with an activity to install, upgrade and roll back nginx on EKS. |
| 6 | 3.12 | Package Manager for Container 2 | Covers creating, templating, packaging and versioning a custom Helm chart, storing it in a chart repository and deploying it to EKS. |
| 6 | CO | Coaching 21 | Fixes a WordPress manifest to connect to an existing MySQL database on EKS, then packages it as a reusable Helm chart. |
| 7 | 3.13 | CICD for Container 1 | Contrasts push-based and pull-based CD, introducing GitOps and Argo CD's architecture and sync model for Kubernetes deployments. |
| 7 | 3.14 | CICD for Container 2 | Goes deeper on Argo CD with sync policies, rollbacks, Helm and Kustomize sources, multi-tenant projects and RBAC, and troubleshooting. |
| 7 | CO | Coaching 22 | Uses PVCs, StorageClasses and reclaim policies to provision EBS volumes on EKS, tests access modes and data persistence, and shares a scratch volume with sidecars. |
| 8 | 3.15 | Architecture & Tool Review | Reviews architecture styles and tool choices for compute, CI/CD, IaC, observability and security, plus Day 0/1/2 operations, ADRs and internal developer platforms. |
| 8 | 3.16 | Case Study & Capstone Prep | |
| 8 | CO | Coaching 23 - Consultation & Review | |
