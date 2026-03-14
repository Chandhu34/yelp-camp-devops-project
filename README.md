
# End-to-End DevOps Implementation of YelpCamp Application

## Project Overview
This project demonstrates a complete **DevOps implementation of the YelpCamp full-stack application** using modern DevOps tools and AWS cloud infrastructure.
The main objective of this project is to automate application delivery using **CI/CD pipelines, containerization, infrastructure as code, Kubernetes orchestration, and monitoring**.
The DevOps implementation was completed in **three deployment stages** to simulate a real-world production pipeline.

-------------------------------------------------------------------

# Deployment Journey
The application was deployed in **three progressive stages**.
## Stage 1 — Local Application Deployment

The application was first deployed and tested on a **local development server** to validate functionality.
This stage involved:
* Installing application dependencies
* Configuring MongoDB Atlas database connection
* Integrating Mapbox for location services
* Integrating Cloudinary for image storage
* Running the application locally

This ensured the application worked correctly before introducing DevOps automation.

--------------------------------------------------------------------

## Stage 2 — CI/CD Pipeline and Containerization

After validating the application locally, a **CI/CD pipeline was implemented using Jenkins**.
This stage automated the build and containerization process.
Pipeline stages include:
* Code checkout from GitHub
* SonarQube code quality analysis
* Quality gate validation
* Docker image build
* Trivy security vulnerability scanning
* Docker image push to DockerHub

The application was then executed inside **Docker containers**.

-------------------------------------------------------------

## Stage 3 — Cloud Deployment using AWS Infrastructure

In the final stage, the application was deployed on **AWS cloud infrastructure using Terraform and Kubernetes**.
Infrastructure provisioning includes:
* AWS EKS Kubernetes cluster
* Worker node groups
* Networking configuration
* IAM roles and permissions

The application was deployed using Kubernetes manifests and exposed through an **AWS Load Balancer**.

------------------------------------------------------------------

# Application Repository

The application source code is hosted in the following repositories.

Application Repository
https://github.com/Chandhu34/3-Tier-Full-Stack-yelp-camp.git

Infrastructure Repository
https://github.com/Chandhu34/k8s-project.git

This repository focuses only on the **DevOps implementation**.

------------------------------------------------------------------------------

# DevOps Architecture

The system follows a complete DevOps workflow.
Developer pushes code to GitHub.
GitHub triggers the Jenkins pipeline.
The pipeline performs:
* Code checkout
* SonarQube code quality analysis
* Docker image build
* Trivy security scanning
* Docker image push to DockerHub
Terraform provisions AWS infrastructure including the EKS cluster.
Kubernetes deploys the application inside the cluster.
Prometheus collects metrics and Grafana visualizes monitoring dashboards.
-------------------------------------------------------

# Tools and Technologies
## DevOps Tools
Jenkins

Docker
Kubernetes
Terraform
Helm
## Monitoring
Prometheus
Grafana
Node Exporter
## Security and Code Quality
SonarQube
Trivy
## Cloud Infrastructure
AWS EC2
AWS EKS
AWS Load Balancer
## Database and Third-Party Services
MongoDB Atlas
Mapbox
Cloudinary

-----------------------------------------------------------

# CI/CD Pipeline Workflow

1. Developer pushes code to GitHub
2. Jenkins pipeline is triggered automatically
3. SonarQube performs static code analysis
4. Quality gate validation ensures code quality
5. Docker builds the application container image
6. Trivy scans the image for vulnerabilities
7. Docker image is pushed to DockerHub
8. Terraform provisions AWS infrastructure
9. Kubernetes deploys the application to EKS
10. Prometheus collects application and cluster metrics
11. Grafana visualizes monitoring dashboards

--------------------------------------------------------------------

# Infrastructure Provisioning
Terraform provisions the following AWS resources:
* AWS EKS Cluster
* Worker Node Group
* Networking configuration
* IAM roles and policies

-----------------------------------------------------------

# Kubernetes Deployment
The application is deployed using the following Kubernetes resources:
* Namespace
* ServiceAccount
* Role and RoleBinding
* Secrets
* Deployment
* Service
* Horizontal Pod Autoscaler
* Pod Disruption Budget

----------------------------------------------------------------------

# Monitoring
Monitoring is implemented using **Prometheus and Grafana**.
Prometheus collects metrics from the Kubernetes cluster including:
* Node metrics
* Pod metrics
* Cluster health
* CoreDNS metrics
Grafana visualizes these metrics through interactive dashboards.

----------------------------------------------------------------------------

# Screenshots

Screenshots of the working system are available in the **screenshots** folder.

These include:

* Jenkins CI/CD Pipeline
* SonarQube Scan Results
* DockerHub Image Repository
* Terraform Infrastructure Deployment
* AWS EKS Cluster
* Kubernetes Pods and Services
* Grafana Monitoring Dashboards
* Application UI

----------------------------------------------------------------

# Key DevOps Concepts Demonstrated

* CI/CD Pipeline Automation
* Containerization with Docker
* Infrastructure as Code using Terraform
* Kubernetes Orchestration
* Observability with Prometheus and Grafana
* Secure Secrets Management
* Cloud Native Deployment

-----------------------------------------------------------------

# Author

Dasari Chandana

Aspiring DevOps Engineer

