---
layout: post
title: "Automating EKS Node Rotation for AMI Releases"
date: 2021-08-03 10:00:00
description: "How we automated our node rotation process for new AMI releases and built open source tools to eliminate toil."
tags: [kubernetes, eks, automation, devops]
author: Stavros Foteinopoulos
---

This article was originally published on the [Mattermost Engineering Blog](https://mattermost.com/blog/automate-eks-node-rotation/).

## The Challenge of Toil

In the world of Site Reliability Engineering, one of our primary goals is to reduce toil - the manual, repetitive work that tends to scale linearly with service growth. Our journey to automate node rotation for AMI releases exemplifies this mission.

## Key Challenges We Faced

1. **Limited Flexibility in Kops**: The sequential node rotation in Kubernetes Operations (kops) wasn't meeting our needs for flexible, environment-specific handling.
2. **EKS Automation Gaps**: AWS EKS clusters lacked automated node rotation capabilities for new AMI releases.

## Our Solution

We developed a comprehensive solution combining existing tools with new implementations:

### Tools and Implementation
- Created a flexible node rotation library (rotator)
- Integrated with our cloud provisioner for kops clusters
- Developed rotatorctl CLI tool for EKS clusters
- Implemented GitLab pipelines for automated AMI releases

### Workflow Improvements
For kops clusters:
- Automated new AMI deployment
- Managed installation traffic during upgrades
- Ensured cluster stability monitoring

For AWS EKS clusters:
- Automated AMI updates in Launch configurations
- Implemented controlled node rotation
- Maintained service availability during updates

## Impact and Benefits

This automation initiative:
- Reduced manual intervention from 2-3 people to automated processes
- Cut down rotation time from 2-8 hours to minimal oversight
- Enabled more frequent security updates
- Improved overall infrastructure reliability

---

*This post summarizes our detailed engineering blog post. For complete technical details and implementation specifics, please visit the [original article](https://mattermost.com/blog/automate-eks-node-rotation/).* 