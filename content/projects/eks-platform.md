---
title: "EKS platform from scratch"
date: 2020-05-01
description: "Designed VPC/CIDR layout, networking and RBAC for production EKS; later fully automated across environments."
tags: ["aws", "eks", "kubernetes", "iac"]
---

**Problem:** a new microservices platform needed Kubernetes on AWS, with nothing in place.

**Built:**
- VPC and CIDR planning, subnet groups, NAT gateways sized for EKS.
- EKS clusters with eksctl; RBAC for developer access to non-prod.
- Later: full IaC automation of EKS and add-ons across environments; Prometheus monitoring for clusters and nodes.

**Result:** repeatable clusters per environment instead of hand-built ones.
