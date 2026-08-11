# OCI Networking Analysis

## Overview

## Overview

I created this repository after being accepted into the Oracle ACE Apprentice Program to document my learning and understanding of Oracle Cloud Infrastructure networking.

The repository explains the core OCI networking components, including Virtual Cloud Networks, public and private subnets, route tables, gateways, Security Lists, and Network Security Groups.

My main learning from this exercise is that OCI networking should not be viewed as separate components. VCNs, subnets, route tables, gateways, and security rules need to work together to control traffic flow and support a secure cloud design.

This repository is based on my own learning and documentation. No client-confidential, proprietary, or project-specific information is included.

---

## Why I Created This

Networking is one of the first areas to understand before deploying workloads in the cloud.
In OCI, the network design decides how resources communicate, how internet access is controlled, and how private workloads are protected. As part of my learning, I wanted to break this down into small topics so that another learner can follow the same flow.

---

## Product Used

Oracle Cloud Infrastructure Networking

---

## Topics Covered

This repository covers:

- Virtual Cloud Network
- Public and private subnets
- Route tables
- Internet Gateway
- NAT Gateway
- Service Gateway
- Dynamic Routing Gateway
- Security Lists
- Network Security Groups
- Basic traffic flow in OCI

---

## Simple Architecture Flow

```mermaid
flowchart TD
    A[Internet] --> B[Internet Gateway]
    B --> C[VCN]
    C --> D[Public Subnet]
    D --> E[Load Balancer or Public Resource]
    C --> F[Private Subnet]
    F --> G[Application Server]
    F --> H[NAT Gateway for outbound internet access]
    F --> I[Service Gateway for private OCI service access]

    C --> J[Route Tables]
    C --> K[Security Lists / NSGs]
```

This is a simple learning example. In a real implementation, the design may change based on security, application, integration, and business requirements.

---

## What I Learned

The key learning from this exercise is that OCI networking is not only about creating a VCN or subnet.
A proper network design depends on how routing, gateways, and security controls are configured together. A subnet may be public or private, but traffic behavior is controlled through route tables, gateways, security lists, and network security groups.
This helped me understand OCI networking from a traffic-flow and design perspective.

---

## Confidentiality Note
All examples in this repository are based on my own learning and documentation. No client-confidential, proprietary, or project-specific information is included.

---

## Oracle ACE Apprentice Note

I created this repository after being accepted into the Oracle ACE Apprentice Program as part of my product usage learning and contribution journey.
