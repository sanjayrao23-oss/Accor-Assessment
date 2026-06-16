## Accor Assessment

## Overview

This repository contains the solution for the Accor SRE assessment.

## Architecture

User → Route53 → CloudFront → AWS WAF → ALB → Ingress → Service → EKS Pods

## Components

- Amazon EKS
- Redis
- RDS Multi-AZ
- HPA
- Cluster Autoscaler / Karpenter
- Datadog
- Prometheus
- Grafana

## Repository Structure

### terraform

Infrastructure provisioning:

- VPC
- Subnets
- ALB
- EKS
- RDS
- Redis

### kubernetes

Application deployment:

- Namespace
- Deployment
- Service
- Ingress
- HPA
- PDB

## High Availability

- Multi-AZ worker nodes
- Multi-AZ RDS
- HPA
- Cluster Autoscaler/Karpenter
- Redis caching

## Observability

- CloudWatch
- Prometheus
- Grafana
- Datadog
