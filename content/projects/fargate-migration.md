---
title: "EC2 → ECS Fargate with zero-downtime canaries"
date: 2025-06-01
description: "Migrated production APIs off EC2 to ECS Fargate behind API Gateway canary deployments; compute baseline down >95%."
tags: ["aws", "ecs", "finops", "canary"]
---

**Problem:** always-on EC2 capacity for production APIs, paid for around the clock.

**Built:**
- ECS Fargate services replacing the EC2 fleet.
- API Gateway canary deployments to shift traffic gradually, with instant rollback.
- Production EKS/Karpenter clusters for workloads that stayed on Kubernetes.

**Result:** compute baseline cut by **over 95%**, no downtime during the cutover.
