
# ☁️ AWS Cloud Essentials

<p align="center">
  <img src="https://img.shields.io/badge/AWS-Cloud%20Essentials-orange?style=for-the-badge&logo=amazonaws" />
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Learning-Journey-blue?style=for-the-badge" />
</p>

## 📖 Overview

This repository contains my notes, labs, and learning outcomes from studying **Amazon Web Services (AWS) Cloud Essentials**.

The goal of this repository is to document my progress in cloud computing while building a strong understanding of AWS core concepts, cloud architecture, security, and global infrastructure.This repository serves as my personal cloud computing knowledge base and portfolio, documenting my hands-on AWS learning journey through notes, labs, projects, and practical exercises.

---


# Module 1️⃣


## 🎯 Learning Objectives

Through this module, I learned how to:

* Understand Cloud Computing fundamentals
* Explore AWS Global Infrastructure
* Differentiate Regions and Availability Zones
* Understand High Availability and Fault Tolerance
* Learn the AWS Shared Responsibility Model
* Apply cloud concepts to real-world business scenarios

---

## 🌎 AWS Global Infrastructure

AWS operates one of the largest cloud infrastructures in the world.

### AWS Regions

AWS Regions are geographically separated locations where AWS operates data centers.

Examples include:

* US East (N. Virginia)
* Europe (Ireland)
* Asia Pacific (Singapore)

Organizations deploy resources in Regions closest to their users to reduce latency and improve performance.

---

### Availability Zones (AZs)

Each AWS Region contains multiple Availability Zones.

Availability Zones are:

* Physically separated
* Independently powered
* Independently networked
* Designed for fault isolation

Using multiple Availability Zones increases application reliability and resilience.

---

## 🔄 High Availability & Fault Tolerance

AWS infrastructure is designed to provide:

### High Availability

Applications remain accessible even if part of the infrastructure experiences issues.

### Fault Tolerance

Services continue operating despite hardware failures or outages.

### Best Practice

Deploy resources across multiple Availability Zones to ensure redundancy and minimize downtime.

---

## 🔐 AWS Shared Responsibility Model

Security in AWS follows a **Shared Responsibility Model**.

### AWS Responsibilities

AWS is responsible for:

* Physical security
* Data centers
* Hardware infrastructure
* Networking infrastructure
* Global cloud services

### Customer Responsibilities

Customers are responsible for:

* Data security
* Identity and access management
* Account permissions
* Client-side encryption
* Security configurations

### Shared Responsibilities

Depending on the AWS service used, some responsibilities are shared between AWS and the customer.

Examples include:

* Network traffic protection
* Server-side encryption
* Operating system configuration
* Application security



![Module-1](images/module-1.0.png)

---

## 🏢 Real-World Use Case

### Global Ecommerce Expansion

A company based in Seattle wanted to expand its services internationally.

### Challenge

Hosting infrastructure in a single location increased latency for customers in Europe and Asia.

### Solution

The company deployed resources to multiple AWS Regions:

#### 🇮🇪 Ireland Region

Benefits:

* Improved availability
* Reduced latency for European customers
* Increased fault tolerance through multiple Availability Zones

#### 🇸🇬 Singapore Region

Benefits:

* Faster access for Asian customers
* Improved user experience
* Reduced response times

### Result

Using AWS allowed the company to expand globally within minutes instead of spending months or years building physical infrastructure.

---

## 🧠 Key Takeaways

* AWS provides a globally distributed cloud platform.
* Availability Zones improve reliability and uptime.
* Multi-region deployments reduce latency.
* Security is a shared responsibility between AWS and customers.
* Cloud computing enables rapid global scalability.

---
## Quiz Score

![Module-1](images/module-1.1.png)


## 📚 Course Progress

| Module   | Topic                 | Status      |
| -------- | --------------------- | ----------- |
| Module 1 | AWS Cloud Essentials | ✅ Completed |

---

#  Module 2️⃣ : Compute, Scaling & Application Integration


---


## 🎯 Learning Objectives

By completing this module, I learned how to:

* Understand cloud compute resources and Amazon EC2
* Compare AWS compute resources with traditional on-premises infrastructure
* Identify and select appropriate EC2 instance families
* Understand Amazon EC2 pricing models
* Use Amazon Machine Images (AMIs)
* Differentiate scalability from elasticity
* Configure Auto Scaling concepts
* Understand Elastic Load Balancing (ELB)
* Explore event-driven architectures
* Understand Amazon SQS, Amazon SNS, and Amazon EventBridge
* Recognize modern cloud application design patterns

---

## 🖥️ Amazon EC2 (Elastic Compute Cloud)

Amazon EC2 provides scalable virtual servers in the cloud. It enables organizations to deploy applications without purchasing, maintaining, or managing physical hardware.

With EC2, resources can be launched, configured, scaled, and terminated on demand.

### Key Benefits

✅ On-demand compute resources

✅ Rapid deployment

✅ Flexible scaling

✅ Global availability

✅ Pay-as-you-go pricing

✅ Reduced infrastructure costs

---

### Traditional Infrastructure vs AWS EC2

| Traditional Infrastructure    | AWS EC2                    |
| ----------------------------- | -------------------------- |
| Purchase physical servers     | Launch instances on demand |
| Weeks or months to deploy     | Minutes to deploy          |
| High upfront costs            | Pay only for usage         |
| Manual scaling                | Automated scaling          |
| Hardware maintenance required | Managed by AWS             |

---

## ⚙️ EC2 Instance Types

AWS offers specialized instance families optimized for different workloads.

| Instance Family       | Description                              | Common Use Cases                        |
| --------------------- | ---------------------------------------- | --------------------------------------- |
| General Purpose       | Balanced compute, memory, and networking | Web servers, applications, repositories |
| Compute Optimized     | High-performance processors              | HPC, gaming servers, ML inference       |
| Memory Optimized      | Large memory capacity                    | Databases, analytics, caching           |
| Accelerated Computing | GPUs and hardware accelerators           | AI/ML, rendering, graphics              |
| Storage Optimized     | High-speed local storage                 | Data warehousing, big data workloads    |

---

## 🛠️ Managing AWS Resources

AWS services are accessed through APIs and can be managed using several interfaces.

### AWS Management Console

A web-based graphical interface for AWS services.

#### Best For

* Beginners
* Learning AWS
* Manual resource management

---

### AWS Command Line Interface (CLI)

A command-line tool used to manage AWS resources.

#### Benefits

* Automation
* Scripting
* Faster administration
* Infrastructure management

Example:

```bash
aws ec2 describe-instances
```

---

### AWS Software Development Kits (SDKs)

SDKs allow developers to integrate AWS services directly into applications.

#### Supported Languages

* Python
* Java
* JavaScript
* C#
* Go
* PHP

---

## 🔐 EC2 & the Shared Responsibility Model

Amazon EC2 follows the AWS Shared Responsibility Model.

### AWS Responsibility (Security *of* the Cloud)

AWS manages:

* Physical security
* Data centers
* Networking infrastructure
* Hardware maintenance
* Global cloud infrastructure

### Customer Responsibility (Security *in* the Cloud)

Customers manage:

* Operating systems
* Security patches
* User access control
* Security groups
* Firewall rules
* Application security

---

## 📦 Amazon Machine Images (AMIs)

An Amazon Machine Image (AMI) is a preconfigured template used to launch EC2 instances.

### Components of an AMI

* Operating System
* Application software
* Storage configuration
* Architecture settings
* Launch permissions

---

### Types of AMIs

#### AWS Managed AMIs

Provided and maintained by AWS.

#### Marketplace AMIs

Created by third-party vendors and available through AWS Marketplace.

#### Custom AMIs

Created and maintained by users for specific organizational requirements.

---

#### Benefits of AMIs

✅ Faster deployments

✅ Consistent configurations

✅ Reduced setup errors

✅ Easier scaling

✅ Standardized environments

---

## 💰 Amazon EC2 Pricing Models

AWS offers multiple pricing options to optimize costs.

| Pricing Model       | Description                                 |
| ------------------- | ------------------------------------------- |
| On-Demand           | Pay only for resources used                 |
| Reserved Instances  | Up to 75% savings for predictable workloads |
| Savings Plans       | Flexible long-term pricing commitments      |
| Spot Instances      | Up to 90% savings using spare AWS capacity  |
| Dedicated Hosts     | Entire physical server reserved             |
| Dedicated Instances | Hardware isolated to a single account       |

---

## 📈 Scalability vs Elasticity

Although related, scalability and elasticity are different concepts.

### Scalability

The ability of a system to increase resources to handle growth.

#### Vertical Scaling (Scale Up)

Increase the power of existing resources.

```text
2 vCPU → 8 vCPU
4 GB RAM → 32 GB RAM
```

#### Horizontal Scaling (Scale Out)

Add additional servers.

```text
1 Server → 5 Servers
```

---
![Module-2](images/module-2.6.png)

---

## Elasticity

The ability to automatically adjust resources based on demand.

#### Example

```text
High Traffic → Add Resources
Low Traffic → Remove Resources
```

#### Benefits

* Better performance
* Lower operational costs
* Efficient resource utilization
* Automatic resource adjustment

---

## 🔄 Amazon EC2 Auto Scaling

Amazon EC2 Auto Scaling automatically adjusts the number of EC2 instances based on application demand.

### Scaling Methods

#### Dynamic Scaling

Automatically responds to real-time demand changes.

#### Predictive Scaling

Forecasts future traffic and provisions resources before demand increases.

---

## Auto Scaling Group Settings

| Setting          | Purpose                             |
| ---------------- | ----------------------------------- |
| Minimum Capacity | Lowest number of running instances  |
| Desired Capacity | Target number of instances          |
| Maximum Capacity | Highest number of instances allowed |

---
### Minimum Capicity 
![Module-2](images/module-2.8.png)


### Maximum Capacity 
![Module-2](images/module-2.9.png)


---

#### Benefits

✅ High availability

✅ Cost optimization

✅ Improved performance

✅ Reduced operational effort

---

## ⚖️ Elastic Load Balancing (ELB)

Elastic Load Balancing distributes incoming traffic across multiple EC2 instances.

#### Without ELB

```text
Users → Single Server
```

#### With ELB

```text
Users → Load Balancer → Multiple Servers
```

---

#### Benefits

✅ Efficient traffic distribution

✅ High availability

✅ Fault tolerance

✅ Better performance

✅ Simplified scaling

---

#### Common Load Balancing Algorithms

| Method              | Description                         |
| ------------------- | ----------------------------------- |
| Round Robin         | Traffic distributed evenly          |
| Least Connections   | Routes to least busy server         |
| IP Hash             | Routes based on client IP           |
| Least Response Time | Routes to fastest responding server |

---

## 🏗️ Application Architecture Patterns

### Monolithic Architecture

All application components are tightly coupled within a single application.

#### Challenges

* Difficult scaling
* Single point of failure
* Slower deployments
* Reduced flexibility

---

### Microservices Architecture

Application components operate independently and communicate through APIs or events.

#### Benefits

* Independent scaling
* Better fault isolation
* Faster deployments
* Improved resilience
* Easier maintenance

---

## 📡 Amazon EventBridge

Amazon EventBridge is a serverless event bus service that enables event-driven architectures.

Applications can communicate through events without being tightly coupled.

### Example: Food Delivery Application

1. Customer places an order
2. Payment service processes payment
3. Restaurant receives notification
4. Inventory is verified
5. Driver receives delivery request

All actions are triggered automatically through events.

---

## 📨 Amazon SQS (Simple Queue Service)

Amazon SQS is a fully managed message queue service that enables reliable communication between distributed application components.

#### Benefits

* Reliable message delivery
* Decoupled applications
* Fault tolerance
* High scalability
* Message persistence

##### Example

Customer support tickets enter a queue and are processed when agents become available.

---

## 📢 Amazon SNS (Simple Notification Service)

Amazon SNS is a publish-subscribe messaging service used for notifications.

#### Features

* Email notifications
* SMS notifications
* Mobile push notifications
* Multiple subscribers
* Topic-based messaging

##### Example

Subscribers receive notifications for:

* New products
* Promotions
* Security alerts
* Company announcements

Only users subscribed to a topic receive its messages.

---

Quiz score
![Module-2](images/module-2.011.png)

# 📚 Course Progress

| Module   | Topic                                      | Status      |
| -------- | ------------------------------------------ | ----------- |
| Module 1 | AWS Cloud Foundations                      | ✅ Completed |
| Module 2 | Compute, Scaling & Application Integration | ✅ Completed |

---

### ⭐ If you found this repository helpful, feel free to star it!
