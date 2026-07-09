---
title: "Proposal"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 2. </b> "
---

# Sports Field Booking System

## AWS-Based Web Application Deployment Solution

### 1. Executive Summary

The Sports Field Booking System is designed to help users search for sports fields, make online reservations, and manage their booking history through a web-based platform. The system is deployed on AWS using a multi-tier architecture to ensure high availability, security, and scalability.

The architecture uses Amazon ECS to deploy the application as containers, Amazon RDS as the relational database, Redis for caching, Amazon S3 for storing static files and images, Amazon CloudFront for fast content delivery, and Amazon Route 53 for DNS management. The application is protected by AWS WAF, while AWS Certificate Manager provides SSL/TLS certificates.

---

## 2. Problem Statement

### Current Challenges

Many sports facilities still manage reservations using phone calls or paper-based records, resulting in:

- Difficult reservation management.
- Double-booking conflicts.
- No centralized payment or reservation management system.
- Poor scalability as the number of sports fields increases.
- Limited availability during periods of high user traffic.

### Proposed Solution

Deploy the system on AWS using a cloud-native architecture.

Users access the website through Amazon Route 53 and Amazon CloudFront.

CloudFront works together with AWS WAF to accelerate content delivery and protect against web attacks.

Application Load Balancer distributes incoming requests to containers running on Amazon ECS.

The application accesses an Amazon RDS database located in a private subnet.

Redis is used to cache frequently accessed data, reducing database workload.

Images and static assets are stored in Amazon S3.

Amazon ECR stores Docker images for the application.

AWS Secrets Manager securely stores database credentials and application secrets.

Amazon CloudWatch monitors the entire system and sends alerts through Amazon SNS.

### Benefits

- Automatic system scaling.
- High-level security.
- High availability.
- Simplified deployment of new application versions.
- Reduced infrastructure management effort.
- Improved performance through CloudFront and Redis caching.

---

## 3. Solution Architecture

The system is deployed within an Amazon VPC consisting of public and private subnets across two Availability Zones to provide high availability.

The workflow is as follows:

1. Users access the website through Amazon Route 53.

2. Amazon CloudFront delivers content with lower latency.

3. AWS WAF inspects and filters malicious requests.

4. Valid requests are forwarded to the Application Load Balancer.

5. The ALB distributes traffic to containers running on Amazon ECS.

6. Amazon ECS processes the application logic.

7. Data is stored in the primary Amazon RDS database.

8. Redis caches frequently accessed data.

9. Amazon RDS Multi-AZ standby in the second Availability Zone provides failover capability.

10. Amazon S3 stores the frontend application and user-uploaded files.

11. Docker images are stored in Amazon ECR.

12. AWS Secrets Manager securely manages database credentials.

13. Amazon CloudWatch monitors all AWS resources.

14. Amazon SNS sends email notifications to administrators when system issues occur.

![System Architecture](/images/2-Proposal/platform_architecture1.jpg)

### AWS Services Used

- Amazon Route 53
- Amazon CloudFront
- AWS WAF
- AWS Certificate Manager
- Amazon S3
- Amazon VPC
- Public Subnet
- Private Subnet
- NAT Gateway
- Application Load Balancer
- Amazon ECS
- Amazon RDS
- Amazon ElastiCache for Redis
- Amazon ECR
- AWS Secrets Manager
- Amazon CloudWatch
- Amazon SNS

### Component Design

**Edge Layer**

- Amazon Route 53 manages DNS.
- Amazon CloudFront delivers content globally.
- AWS WAF protects the web application.
- AWS Certificate Manager provides SSL/TLS certificates.
- Amazon S3 stores the frontend application and uploaded files.

**Application Layer**

- Application Load Balancer distributes incoming traffic.
- Amazon ECS runs the backend services.
- Amazon ECR stores Docker images.

**Database Layer**

- Amazon RDS Primary Database.
- Amazon RDS Multi-AZ Standby Database.
- Redis Cache.

**Monitoring Layer**

- Amazon CloudWatch monitors system resources.
- Amazon SNS sends email notifications and alerts.

---

## 4. Technical Implementation

### Phase 1

- Requirement analysis.
- Database design.
- AWS architecture design.

### Phase 2

- Create Amazon VPC.
- Configure subnets.
- Deploy NAT Gateway.
- Configure Security Groups.

### Phase 3

- Deploy Amazon ECS.
- Push Docker images to Amazon ECR.
- Configure the Application Load Balancer.

### Phase 4

- Deploy Amazon RDS.
- Configure Redis.
- Configure AWS Secrets Manager.

### Phase 5

- Configure Amazon CloudFront.
- Configure Amazon Route 53.
- Configure AWS WAF.
- Configure AWS Certificate Manager.

### Phase 6

- Configure Amazon CloudWatch.
- Configure Amazon SNS.
- Perform system testing.
- Deploy the system to production.

---

## 5. Implementation Timeline

| Phase | Activities |
|--------|------------|
| Month 1 | System design |
| Month 2 | Backend and database development |
| Month 3 | Deploy Amazon ECS and Amazon RDS |
| Month 4 | System testing and production deployment |

---

## 6. Estimated Budget

The estimated costs include:

- Amazon ECS
- Amazon RDS
- Amazon ElastiCache
- Amazon CloudFront
- Amazon Route 53
- Amazon S3
- NAT Gateway
- Application Load Balancer
- Amazon CloudWatch
- Amazon SNS

The total cost depends on the ECS configuration, database size, and actual traffic volume.

---

## 7. Risk Assessment

### Risks

- Amazon ECS service failure.
- Database overload.
- Redis failure.
- DDoS attacks.
- Database storage exhaustion.

### Mitigation Strategies

- Deploy ECS across multiple Availability Zones.
- Enable Amazon RDS Multi-AZ.
- Use Amazon CloudFront to reduce backend traffic.
- Protect the application with AWS WAF.
- Monitor the system using Amazon CloudWatch and send alerts through Amazon SNS.

---

## 8. Expected Outcomes

- Stable 24/7 system operation.
- Scalability to support increasing numbers of users.
- Strong security and data protection.
- Faster deployment using Docker containers and Amazon ECS.
- High database availability through Amazon RDS Multi-AZ.
- Easy maintenance and future upgrades.