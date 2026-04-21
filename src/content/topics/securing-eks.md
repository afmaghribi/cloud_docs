---
title: "Securing EKS Clusters"
description: "Best practices and guidelines for securing Amazon Elastic Kubernetes Service."
order: 1
---

Securing an EKS cluster requires a multi-layered approach, addressing both the control plane and the data plane.

## 1. IAM Integration

Ensure that IAM roles for service accounts (IRSA) are properly configured. Never use node instance roles for your application pods.

## 2. Network Policies

By default, pods are non-isolated. Use Kubernetes Network Policies to restrict traffic between pods.

## 3. Container Security

- Scan images for vulnerabilities.
- Run containers as non-root users.
- Make root filesystems read-only where possible.

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Dictum fusce ut placerat orci nulla pellentesque dignissim enim.