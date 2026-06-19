🚀 Built a Production-Grade, Highly Available Deployment Pipeline on AWS (ECS + Fargate) with Full CI/CD, Monitoring & Backups
Proud to share a major hands-on project I completed: designing and deploying a highly available Employee Management REST API on AWS, fully automated end-to-end using GitLab CI/CD, CloudFormation, and best-practice cloud architecture.
This wasn’t just about deploying an app — it was about building a reliable, secure, observable, fault-tolerant system, similar to what modern SaaS companies run in production.
🧩 🔹 Project Highlights
1️⃣ Infrastructure as Code (CloudFormation)
Provisioned a complete production VPC:
Multi-AZ Public & Private Subnets
NAT Gateway + IGW
ECS Cluster (Fargate)
ALB + Target Groups
ECR Repository
S3 Buckets (Backups/Static Assets)
IAM Roles, Security Groups, Logs
Parameterized ECS Task Definition for seamless image updates
2️⃣ CI/CD Pipeline (GitLab)
Automated pipeline with stages:
Build Docker image
Test API logic
Push to ECR
Deploy via CloudFormation updates
Zero-downtime ECS service rollout
3️⃣ Application Layer (FastAPI)
A lightweight Employee CRUD API containerized using:
Dockerfile
.dockerignore
Supports both MongoDB or file-based DB for demo mode
4️⃣ Database + Backups
Instead of RDS (to reduce cost):
Deployed MongoDB on EC2 with attached EBS
Automated daily EBS snapshot → S3 backup workflow
Documented restore procedure
5️⃣ CDN + DNS
Configured CloudFront for global caching
Route53 domain mapping
SSL via AWS ACM
Significantly faster response times globally
6️⃣ Monitoring + Observability
Implemented cloud-native monitoring:
CloudWatch metrics, dashboards & custom alarms
CloudTrail for API auditing
ECS Task Logs shipped to CloudWatch
#aws #gitlab #devops #cloudfront

# "for security,i edited the urls in the ppt"
