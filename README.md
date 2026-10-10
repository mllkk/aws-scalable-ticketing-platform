# AWS Ticket Sales Platform

A hands-on AWS cloud project designed to simulate the infrastructure of a high-traffic concert ticket sales platform.

The main goal of this project is to learn and demonstrate how AWS services can be combined to build a scalable, secure and resilient distributed application.

The project is developed incrementally. Each phase introduces a new AWS service or architectural concept and documents the implementation, testing process and lessons learned. You can find the roadmap at the very bottom of the README page. 

📬 Stay Updated: To read the development blogs and track our progress phase by phase, check out the Issues tab.

## 🎯 Project Goal

The platform simulates a high-traffic concert ticket sales system where a large number of users may attempt to access the application and purchase tickets simultaneously.

The project focuses on two main technical challenges:

### 1. Handling High Traffic 🚦

The system should remain responsive and operational when traffic increases significantly.

The architecture uses AWS services such as: Application Load Balancer, EC2, Auto Scaling and CloudWatch to distribute traffic, dynamically adjust application capacity and monitor the health of the infrastructure.

Load testing will be performed to observe how the infrastructure behaves under increasing traffic and whether Auto Scaling can provide additional capacity when required.

### 2. Preventing Concurrent Seat Purchases ⏳

The second challenge is maintaining data consistency when multiple users attempt to purchase the same seat at the same time.

The system uses DynamoDB conditional writes to ensure that only one request can successfully reserve the seat.

Together, these components demonstrate how a distributed AWS architecture can handle both increased traffic and concurrent transactions without compromising application availability or data consistency.

## 📐 Architecture 
The target architecture is based on the following flow:

<img width="1148" height="628" alt="Ekran görüntüsü 2026-10-04 182540" src="https://github.com/user-attachments/assets/32760ed9-5bc2-4ba1-95bd-b70f2e655a96" />

Tech With Soleyman. (Jul 9, 2026). Learn 97% of AWS in Under 30 Minutes (Beginner to Pro) [Video]. YouTube. [https://youtu.be/ujeEIbu_JxE?si=9i6psJB74ymXol8i].

## 🚧 Project in progress

* 🌐 **Phase 01** - VPC & Network Architecture
* 💻 **Phase 02** - EC2 Backend Application
* ⚖️ **Phase 03** - Application Load Balancer
* 📈 **Phase 04** - EC2 Auto Scaling
* 🧪 **Phase 05** - Auto Scaling Load Test with k6
* 🐘 **Phase 06** - RDS PostgreSQL
* ⚡ **Phase 07** - DynamoDB Concurrent Seat Purchase
* 📥 **Phase 08** - SQS & Lambda Asynchronous Processing
* 📦 **Phase 09** - S3 & CloudFront Frontend
* 🗺️ **Phase 10** - Route 53 DNS
* 🔐 **Phase 11** - IAM & Security Groups
* 📊 **Phase 12** - CloudWatch Monitoring
* 🏗️ **Phase 13** - Terraform Infrastructure as Code
* 🤖 **Phase 14** - Ansible Automation
* 🐳 **Phase 15** - Docker
* ☸️ **Phase 16** - Kubernetes
* 🚀 **Phase 17** - CI/CD with GitHub Actions
