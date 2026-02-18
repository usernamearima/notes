# Cloud Computing Basics

These notes cover fundamental cloud computing concepts.
The focus is on understanding how cloud environments work
and what security implications they introduce.

---

## 1. What Is Cloud Computing

Cloud computing means using computing resources
over the internet instead of on local hardware.

Resources provided by the cloud:
- servers
- storage
- databases
- networking
- applications

You do not manage physical hardware.
You rent resources on demand.

---

## 2. Why Cloud Exists

Cloud computing is used because it:
- scales easily
- reduces hardware costs
- enables rapid deployment
- allows global access

Organizations can grow or shrink infrastructure
without buying new machines.

---

## 3. Cloud Service Models

### IaaS – Infrastructure as a Service
You manage:
- operating systems
- applications
- configurations

The provider manages:
- physical servers
- networking
- storage

Example use:
- virtual machines in the cloud

---

### PaaS – Platform as a Service
You manage:
- applications
- data

The provider manages:
- operating system
- runtime
- infrastructure

Example use:
- application hosting platforms

---

### SaaS – Software as a Service
You manage:
- user access
- configuration

The provider manages:
- everything else

Example use:
- email services
- cloud office tools

---

## 4. Shared Responsibility Model

Cloud security is based on shared responsibility.

The cloud provider is responsible for:
- physical data centers
- underlying hardware
- base infrastructure

The customer is responsible for:
- user access
- data
- configurations
- permissions

Many cloud security issues come from
customer misconfiguration.

---

## 5. Cloud Identity and Access Management (IAM)

IAM controls:
- who can access resources
- what actions they can perform

IAM uses:
- users
- roles
- policies

Poor IAM configuration is a major cloud risk.

---

## 6. Cloud Networking (High-Level)

Cloud networks are virtual.

Key components:
- virtual networks
- subnets
- routing rules
- security groups / firewall rules

Networking controls:
- which systems can communicate
- what ports are allowed
- traffic direction

---

## 7. Cloud Storage

Cloud storage stores data remotely.

Common storage types:
- object storage
- block storage
- file storage

Security risks include:
- public data exposure
- weak access controls
- misconfigured permissions

---

## 8. Logging and Monitoring in the Cloud

Cloud platforms provide logging services.

Logs may include:
- access logs
- authentication events
- configuration changes
- network traffic

Logging is critical for:
- detecting attacks
- incident response
- compliance

---

## 9. Common Cloud Security Risks

Typical cloud security issues:
- exposed storage buckets
- overly permissive IAM roles
- weak authentication
- lack of monitoring
- insecure APIs

Most issues are configuration-related,
not cloud provider failures.

---

## 10. Cloud in Cybersecurity

Cloud environments are used for:
- hosting applications
- storing sensitive data
- running security tools
- lab environments

Understanding cloud fundamentals
is essential for modern cybersecurity roles.

---

## Key Takeaways

- cloud provides on-demand resources
- service models define responsibility
- security is shared between provider and customer
- IAM is critical to cloud security
- misconfiguration is the main risk
- logging enables detection and response
