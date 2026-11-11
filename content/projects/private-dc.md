---
title: "Private data center to production"
date: 2024-03-01
description: "Private cloud in a colo: Ansible + Terraform VM automation for GitLab runners and Jenkins workers; provisioning 75% faster."
tags: ["datacenter", "kubernetes", "ansible", "terraform"]
---

**Problem:** firmware build infrastructure needed its own data center, on a closed network.

**Built:**
- VM builds on vCenter/ESXi; Kubernetes with kubeadm; Dell ECS object storage; FortiGate/FortiADC networking.
- Ansible for VM configuration (compliance + closed-network settings); Terraform for VM lifecycle.
- Monitoring for the data center and the build pipelines running on it.

**Result:** in production; provisioning streamlined by **75%**.
