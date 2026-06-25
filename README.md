
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


### ⭐ If you found this repository helpful, feel free to star it!
