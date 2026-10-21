# ☁️ 100 Days of Cloud Challenge

My hands-on journey through **KodeKloud's 100 Days of Cloud Challenge**, focused on AWS.

This repository documents every task I complete — with objectives, steps taken, AWS services used, and key learnings. It serves as my public cloud engineering portfolio.

## 🎯 Goal
- Build real, job-ready AWS skills through daily hands-on labs
- Document each task for transparency and review
- Create a verifiable portfolio for recruiters and hiring managers

## 📊 Progress

| Day | Task | AWS Services | Status |
|-----|------|--------------|--------|
| 01 | Create an RSA key pair (`devops-kp`) | EC2 | ✅ |
| 02 | Create security group (`datacenter-sg`) | EC2, VPC | ✅ |
| 03 | Create subnet (`devops-subnet`) | VPC | ✅ |
| 04 | Enable versioning on S3 (`datacenter-s3-644460639`) | S3 | ✅ |
| 05 | Create EBS volume (`nautilus-volume`) | EC2 (EBS) | ✅ |
| 06 | Launch EC2 instance (`xfusion-ec2`) | EC2 | ✅ |
| 07 | Change instance type (`nautilus-ec2` t2.micro → t2.nano) | EC2 | ✅ |
| 08 | Enable stop protection for `datacenter-ec2` | EC2 | ✅ |
| 09 | Enable termination protection for `devops-ec2` | EC2 | ✅ |
| 10 | Attach Elastic IP (`nautilus-ec2-eip`) to `nautilus-ec2` | EC2 (EIP) | ✅ |
| 11 | Attach ENI (`devops-eni`) to `devops-ec2` | EC2 (ENI) | ✅ |
| 12 | Attach EBS volume (`datacenter-volume`) to `datacenter-ec2` | EC2 (EBS) | ✅ |
| 13 | Create AMI (`datacenter-ec2-ami`) from `datacenter-ec2` | EC2 (AMI) | ✅ |
| 14 | Terminate EC2 instance (`devops-ec2`) | EC2 | ✅ |
| 15 | Create snapshot (`nautilus-vol-ss`) from `nautilus-vol` | EC2 (EBS Snapshot) | ✅ |
| 16 | Create IAM user (`iamuser_yousuf`) | IAM | ✅ |
| 17 | Create IAM group (`iamgroup_ravi`) | IAM | ✅ |
| 18 | Create IAM policy (`iampolicy_mariyam`) | IAM | ✅ |
| 19 | Attach IAM policy (`iampolicy_jim`) to `iamuser_jim` | IAM | ✅ |
| 20 | Create IAM role (`iamrole_rose`) for EC2 | IAM | ✅ |
| 21 | Launch EC2 (`nautilus-ec2`) and associate EIP (`nautilus-eip`) | EC2 (EIP) | ✅ |
| 22 | Configure passwordless SSH for `root` on `datacenter-ec2` | EC2 | ✅ |
| 23 | S3 Bucket Data Migration (`devops-s3` → `devops-sync`) | S3 | ✅ |
| 24 | Application Load Balancer + Target Group setup | EC2 (ALB) | ✅ |
| 25 | Create CloudWatch alarm (devops-alarm) for CPU | CloudWatch | ✅ |
| 26 | Configure EC2 as Nginx web server via User Data | EC2 | ✅ |
| 27 | Configure public VPC with EC2 instance (`nautilus-pub-ec2`) | VPC, EC2 | ✅ |
| 28 | Create private ECR repository (`nautilus-ecr`) and push Docker image | ECR | ✅ |
| 29 | VPC Peering between Default and Private VPCs | VPC, EC2 | ✅ |
| 30 | Configure NAT Instance (`devops-nat-instance`) for private subnet | VPC, EC2, S3 | ✅ |
| 31 | Provision private RDS instance (`datacenter-rds`) | RDS | ✅ |
| 32 | RDS Snapshot and Restore (xfusion-snapshot-restore) | RDS | ✅ |
| 33 | Create Lambda function (`datacenter-lambda`) | Lambda, IAM | ✅ |

### 🛠️ Terraform Progress

| # | Task | Status |
|---|------|--------|
| 1 | Create RSA key pair (`xfusion-kp`) | ✅ |
| 2 | *Coming soon* | ⬜ |
| 3 | *Coming soon* | ⬜ |

## 🛠️ Skills Covered
- **Compute**: EC2, Lambda
- **Storage**: S3, EBS
- **Networking**: VPC, Subnets, Security Groups
- **Database**: RDS, DynamoDB
- **IAM & Security**: Users, Roles, Policies, Key Pairs
- **Infrastructure as Code**: CloudFormation, Terraform
- **Containers**: Docker, ECS, EKS

## 📂 Repository Structure
```text
100-days-of-cloud/
├── Day-01/
│   ├── README.md
│   └── keypair-created.png
├── Day-02/
│   ├── README.md
│   └── sg-inbound-rules.png
├── Day-03/
│   ├── README.md
│   └── devops-subnet.png
├── Day-04/
│   ├── README.md
│   └── s3-versioning.png
├── Day-05/
│   ├── README.md
│   └── nautilus-volume.png
├── Day-06/
│   ├── README.md
│   ├── xfusion-kp-keypair.png
│   ├── xfusion-ec2-launch.png
│   └── xfusion-ec2-list.png
├── Day-07/
│   ├── README.md
│   └── nautilus-ec2-rightsized.png
├── Day-08/
│   ├── README.md
│   └── datacenter-ec2-stop-protection.png
├── Day-09/
│   ├── README.md
│   └── devops-ec2-termination-protection.png
├── Day-10/
│   ├── README.md
│   ├── Allocate-Elastic-IP-address.png
│   └── nautilus-ec2-eip-attached.png
├── Day-11/
│   ├── README.md
│   └── devops-eni-attached.png
├── Day-12/
│   ├── README.md
│   └── datacenter-volume-attached.png
├── Day-13/
│   ├── README.md
│   ├── datacenter-ec2-ami-creation.png
│   └── datacenter-ec2-ami-available.png
├── Day-14/
│   ├── README.md
│   └── devops-ec2-terminated.png
├── Day-15/
│   ├── README.md
│   └── nautilus-vol-ss.png
├── Day-16/
│   ├── README.md
│   └── iamuser_yousuf.png
├── Day-17/
│   ├── README.md
│   └── iamgroup_ravi.png
├── Day-18/
│   ├── README.md
│   └── iampolicy_mariyam.png
├── Day-19/
│   ├── README.md
│   └── iamuser_jim-policy-attached.png
├── Day-20/
│   ├── README.md
│   └── iamrole_rose.png
├── Day-20/
│   ├── README.md
│   └── nautilus-eip-attached.png
├── Day-22/
│   ├── README.md
│   └── datacenter-ec2-ssh-root.png
├── Day-23/
│   ├── README.md
│   └── s3-migration-verification.png
├── Day-24/
│   ├── README.md
|   ├── devops-sg.png
|   ├── devops-tg.png
|   ├── devops-alb.png
|   └── devops-ec2.png
├── Day-25/
│   ├── README.md
|   ├── devops-alarm-created.png
├── Day-26/
│   ├── README.md
|   ├── xfusion-ec2-nginx.png
├── Day-27/
│   ├── README.md
│   ├── nautilus-pub-ec2-details.png
│   └── nautilus-public-rt.png
├── Day-28/
│   ├── README.md
│   └── nautilus-ecr-image.png
├── Day-29/
│   ├── README.md
│   └── xfusion-vpc-peering-ping.png
├── Day-30/
│   ├── README.md
|   ├── pub-subnet.png
│   ├── nat-sg.png
|   ├── nat-iptables-setup.png
│   └── nat-instance-s3-success.png
├── Day-31/
│   ├── README.md
│   └── datacenter-rds-available.png
├── Day-32/
│   ├── README.md
│   └── xfusion-snapshot-restore.png
├── Day-33/
│   ├── README.md
│   ├── datacenter-lambda-test.png
│   └── lambda-execution-role-created.png
├── Terraform/
│   ├── README.md
│   ├── main.tf
│   └── terraform-task1.png
└── README.md (this file)
```


## 🔗 Connect
- **LinkedIn**: https://linkedin.com/in/sidrasoudagar
- **KodeKloud Profile**: https://kodekloud.com/user/sidrasoudagar

---
*Started: September 2026*
