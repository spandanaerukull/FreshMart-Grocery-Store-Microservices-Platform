# FreshMart Grocery Store Microservices Platform

FreshMart is a production-style grocery shopping platform built using a microservices architecture.

This project is based on an open-source microservices application, but it is being customized into a grocery store platform for production-style DevOps learning and interview preparation.

## Project Features

Customers can:

- Browse grocery products
- Search and view product details
- Add grocery items to the cart
- Remove items from the cart
- Complete checkout
- Process payments
- Select delivery options
- Receive order confirmation
- View recommended grocery products
- View promotions and discounts

## Microservices

| Service | Responsibility |
|---|---|
| Frontend | Grocery store web interface |
| Product Catalog | Grocery product information |
| Cart Service | Customer shopping cart |
| Checkout Service | Order processing |
| Payment Service | Payment processing |
| Shipping Service | Grocery delivery calculation |
| Recommendation Service | Recommended grocery products |
| Offers Service | Promotions and discounts |
| Email Service | Order confirmation |
| Redis | Temporary cart storage |

## DevOps Technology Stack

- Git and GitHub
- Docker
- Docker Compose
- Jenkins
- SonarQube
- Trivy
- AWS ECR
- Terraform
- AWS EKS
- Kubernetes
- Helm
- AWS Application Load Balancer
- Prometheus
- Grafana
- CloudWatch
- Centralized logging

## Planned CI/CD Flow

```text
Developer
   |
   v
GitHub
   |
   v
Jenkins CI/CD
   |
   +-- Build and Unit Tests
   +-- SonarQube Code Analysis
   +-- Docker Image Build
   +-- Trivy Security Scan
   +-- Push Images to AWS ECR
   |
   v
AWS EKS
   |
   +-- Kubernetes Deployments
   +-- Services
   +-- ConfigMaps and Secrets
   +-- Ingress and AWS ALB
   |
   v
Public FreshMart Application

