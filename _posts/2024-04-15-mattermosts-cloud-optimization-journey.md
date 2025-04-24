---
layout: post
title: "Mattermost's Cloud Optimization Journey: Pillars of Success"
date: 2024-04-15 10:00:00
description: "A deep dive into Mattermost's transformative journey in cloud optimization, exploring strategic initiatives and future strategies."
tags: [cloud-optimization, finops, aws, cloud-native]
author: Stavros Foteinopoulos, Angelos Kyratzakos
---

This article was originally published on the [Mattermost Engineering Blog](https://mattermost.com/blog/mattermosts-cloud-optimization-journey/).

## Cloud Optimization: Pillars of Success

At Mattermost, we've embarked on a transformative journey in cloud optimization, marked by strategic initiatives and innovative approaches. Here are the key pillars that have guided our success:

### 1. Systematic Cost Tracking
- Established foundation for cloud expense visibility
- Introduced measurable KPIs like Average Production Workspace Cost
- Built advanced monthly cost tracking reports

### 2. Infrastructure Optimization
- Deployed database proxy for efficient multi-tenancy
- Implemented automated cleanup solutions using AWS Lambda
- Created custom cost alerting tools

### 3. Monitoring and Alerting Evolution
- Transitioned to Grafana for unified cost monitoring
- Integrated AWS StackSets for centralized management
- Developed company-wide cost optimization strategies

### 4. Reserved Instance Management
- Adopted Zesty for automated EC2 RI management
- Implemented strategic RDS Reserved Instance planning
- Established yearly evaluation cycles for database needs

## Future Strategies: Embracing ARM/Graviton

Our forward-looking strategy includes:
- Transitioning databases to ARM/Graviton workloads
- Adapting internal services for ARM64 support
- Migrating DNS servers to ARM64 instances
- Planning for hybrid AMD/ARM architecture support

## Lessons Learned: Spot Instances

Our experience with spot instances taught us valuable lessons about balancing cost savings with operational stability. While the potential for savings was attractive, we found that the unpredictability and management complexity didn't align with our operational objectives.

---

*This post is a summary of our detailed engineering blog post. For the complete technical details and implementation specifics, please visit the [original article](https://mattermost.com/blog/mattermosts-cloud-optimization-journey/).* 