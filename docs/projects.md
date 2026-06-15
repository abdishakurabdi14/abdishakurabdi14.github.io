---
layout: default
title: Projects
permalink: /projects/
---

# Projects

## Automated AWS ECS Deployment Pipeline

### Overview

Built an automated cloud deployment pipeline for a containerised Python Flask application using Docker, Terraform, AWS ECS Fargate, Amazon ECR, Application Load Balancer, and GitHub Actions.

The project focuses on automating the process of building, pushing, and deploying a containerised application into AWS using infrastructure as code and CI/CD practices.

### Architecture

<pre>
GitHub Repository
      ↓
GitHub Actions
      ↓
Docker Build
      ↓
Amazon ECR
      ↓
AWS ECS Fargate
      ↓
Application Load Balancer
      ↓
End User
</pre>

### Technologies Used

- AWS ECS Fargate
- Amazon ECR
- Application Load Balancer
- Terraform
- Docker
- GitHub Actions
- OIDC Authentication
- Python
- Flask
- Gunicorn
- Linux

### What I Built

- Containerised a Python Flask application using Docker and Gunicorn.
- Provisioned AWS infrastructure using Terraform.
- Created ECS services, task definitions, IAM roles, security groups, and networking resources.
- Configured an Application Load Balancer to route traffic to the ECS service.
- Built a GitHub Actions workflow to build the Docker image, push it to Amazon ECR, and redeploy the ECS service.
- Implemented OIDC authentication between GitHub Actions and AWS to avoid long-lived access keys.
- Added a `/health` endpoint for load balancer health checks.

### Challenges Solved

- Resolved Docker image architecture mismatch issues.
- Fixed ECS task deployment failures.
- Debugged Application Load Balancer 502 and 503 errors.
- Configured security groups and port mappings correctly.
- Troubleshot IAM and OIDC permission issues.
- Validated deployment availability using ALB health checks.

### Result

The final pipeline allows application changes to be pushed from GitHub, built into a Docker image, stored in Amazon ECR, and deployed automatically to AWS ECS Fargate.

This project strengthened my understanding of cloud infrastructure, containers, CI/CD, AWS networking, IAM, and infrastructure troubleshooting.

---

## Mingle Backend

### Overview

Built and deployed a containerised backend service for a social/event platform using Node.js, Express, MongoDB, JWT authentication, Docker Compose, and Google Cloud.

The project focused on backend API development, authentication, database integration, containerisation, and cloud deployment.

### Architecture

<pre>
Client / Postman
      ↓
REST API
      ↓
Node.js / Express
      ↓
MongoDB
      ↓
Docker Compose
      ↓
Google Cloud VM
</pre>

### Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT Authentication
- bcrypt
- Docker
- Docker Compose
- Google Cloud
- Postman
- GitHub

### What I Built

- Developed REST API endpoints for user authentication and event management.
- Implemented secure password hashing using bcrypt.
- Added JWT-based authentication for protected routes.
- Used MongoDB and Mongoose for database modelling and persistence.
- Containerised the backend using Docker and Docker Compose.
- Deployed and configured the application on a Google Cloud virtual machine.
- Tested API endpoints using Postman.

### Features

- User registration and login.
- Secure password hashing.
- JWT authentication.
- Protected API routes.
- Event creation and viewing.
- Event joining functionality.
- Capacity limits for events.
- Cloud deployment using Google Cloud VM infrastructure.

### Result

The final application demonstrated a complete backend deployment workflow, from API development and authentication to containerisation and cloud hosting.

This project helped strengthen my backend development, Docker, cloud deployment, and API testing skills.
