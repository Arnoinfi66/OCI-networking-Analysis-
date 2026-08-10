# OCI Networking Analysis

## Overview

I created this repository as part of my Oracle ACE Apprentice learning journey to document my hands-on understanding of Oracle Cloud Infrastructure networking.

The focus of this repository is to explain the basic OCI networking components in a simple and practical way. I wanted to understand how VCNs, subnets, gateways, route tables, security lists, and network security groups work together to control traffic flow in OCI.

This is not official Oracle documentation. These are my own learning notes, examples, and observations based on my practice and study of OCI networking.

---

## Why I Created This

Networking is one of the first areas that needs to be understood before deploying workloads in the cloud.

In OCI, the network design decides how resources communicate, how internet access is controlled, and how private workloads are protected. As part of my learning, I wanted to break this down into small topics so that another learner can follow the same flow.

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

```text
Internet
   |
   v
Internet Gateway
   |
   v
VCN
   |
   v
Public Subnet
   |
   v
Load Balancer / Public Resource
   |
   v
Private Subnet
   |
   v
Application Server
