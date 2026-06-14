<img width="995" height="502" alt="image" src="https://github.com/user-attachments/assets/c75f836d-1834-4687-8dbf-3537d84be2a0" /># DevSecOps-Netflix-Project
Complete DevSecOps pipeline for a Netflix Clone featuring SonarQube, Trivy, Jenkins, Docker, Prometheus, Grafana, Amazon EKS, and Argo CD.

# 🚀 Deploying a Secure Netflix Clone with DevSecOps & K8s
### Check out my SOP File ###
## 📌 Overview

This project demonstrates a complete end-to-end DevSecOps implementation for deploying a Netflix Clone application using modern cloud-native technologies and security-first CI/CD practices.

The solution integrates:

✅ Continuous Integration & Continuous Deployment (CI/CD)

✅ Static Code Analysis & Quality Gates

✅ Vulnerability Scanning

✅ Containerization & Image Security

✅ Kubernetes Deployment on Amazon EKS

✅ GitOps with Argo CD

✅ Monitoring & Alerting with Prometheus & Grafana

✅ Automated Email Notifications

---

# 🏗️ Architecture

<img width="2752" height="1536" alt="Architecture Diagram" src="https://github.com/user-attachments/assets/291c6717-a368-4e90-83c9-95d345a0504d" />


### End-to-End Workflow

The deployment pipeline follows a complete DevSecOps lifecycle:

```text
Developer → GitHub → Jenkins Pipeline
                     ↓
       SonarQube Code Analysis
                     ↓
       OWASP Dependency Check
                     ↓
            Trivy Security Scan
                     ↓
          Docker Build & Push
                     ↓
             Amazon EKS
                     ↓
                Argo CD
                     ↓
        Netflix Clone Deployment
                     ↓
     Prometheus + Grafana Monitoring
                     ↓
         Email Notifications
```

---

# 🧠 Real-World Problem Solved

Traditional application deployments often face challenges such as:

❌ Manual deployment processes

❌ Lack of security validation

❌ No centralized monitoring

❌ Configuration drift across environments

❌ Slow feedback loops

❌ Difficult rollback and recovery procedures

This project addresses those challenges by implementing a fully automated DevSecOps workflow with integrated security scanning, monitoring, and GitOps-based deployments.

---

# 🛠️ How I Implemented This (Step-by-Step Summary)

## ☁️ Step 1 — AWS Infrastructure Provisioning

Created AWS EC2 instances to host:

* Jenkins
* SonarQube
* Prometheus
* Grafana
* Argo CD
* Netflix Clone Application

Configured:

* Elastic IP
* Security Groups
* SSH Access via Git Bash

### Outcome

✅ Infrastructure ready for DevSecOps deployment.

---

## 🎬 Step 2 — TMDB API Integration

Configured TMDB API access for dynamic movie metadata.

Used API credentials during Docker image build.

### Outcome

✅ Netflix Clone successfully integrated with TMDB services.

---

## 🐳 Step 3 — Docker Containerization

Built and deployed the Netflix Clone using Docker.

```bash
docker build -t netflix .
docker run -d -p 8888:80 netflix
```

### Outcome

✅ Containerized application running successfully.

---

## 🛡️ Step 4 — SonarQube Code Quality Analysis

Deployed SonarQube and integrated it with Jenkins.

Performed:

* Static Code Analysis
* Code Quality Validation
* Quality Gate Enforcement

### Outcome

✅ Automated code quality verification enabled.

---

## 🔍 Step 5 — Trivy Vulnerability Scanning

Integrated Trivy into the CI/CD pipeline.

Executed:

* Filesystem Scanning
* Container Image Scanning

### Outcome

✅ Security vulnerabilities identified before deployment.

---

## 📦 Step 6 — OWASP Dependency Check

Configured OWASP Dependency Check plugin in Jenkins.

Validated third-party dependencies for known vulnerabilities.

### Outcome

✅ Dependency security validation automated.

---

## ⚙️ Step 7 — Jenkins CI/CD Automation

Configured Jenkins pipeline with:

* GitHub Integration
* SonarQube Analysis
* Dependency Check
* Trivy Scan
* Docker Build
* Docker Push

### Outcome

✅ Fully automated DevSecOps pipeline.

---

## 🚀 Step 8 — Docker Hub Image Publishing

Published container images automatically after successful builds.

### Outcome

✅ Version-controlled container images available for deployment.

---

## 📊 Step 9 — Monitoring & Observability

Implemented monitoring stack using:

### Prometheus

* Metrics Collection
* Target Monitoring

### Node Exporter

* Server Metrics
* Resource Utilization

### Grafana

* Infrastructure Dashboards
* Jenkins Monitoring Dashboards

### Outcome

✅ Real-time visibility into infrastructure and CI/CD operations.

---

## 📧 Step 10 — Email Notification Automation

Configured Jenkins email notifications using:

* Gmail SMTP
* Extended Email Plugin

Notifications include:

* Build Status
* Security Scan Reports
* Trivy Scan Attachments

### Outcome

✅ Instant deployment feedback delivered to stakeholders.

---

## ☸️ Step 11 — Amazon EKS Deployment

Provisioned:

* Amazon EKS Cluster
* Managed Node Groups

Configured:

* AWS CLI
* kubectl
* eksctl

### Outcome

✅ Production-ready Kubernetes environment deployed.

---

## 🔄 Step 12 — GitOps Deployment with Argo CD

Installed Argo CD on Amazon EKS.

Connected Git repository containing Kubernetes manifests.

Implemented:

* Continuous Synchronization
* Automated Deployment Updates
* GitOps Workflow

### Outcome

✅ Declarative Kubernetes deployments managed through Git.

---

# 📈 Monitoring Stack

| Component           | Purpose            |
| ------------------- | ------------------ |
| Prometheus          | Metrics Collection |
| Node Exporter       | Server Metrics     |
| Grafana             | Visualization      |
| Jenkins Plugin      | CI/CD Monitoring   |
| Email Notifications | Alerting           |

---

# 🏆 Project Outcome Summary

| Implementation Area                                           | Status                 |
| ------------------------------------------------------------- | ---------------------- |
| AWS Infrastructure & Docker Deployment                        | ✔ Completed            |
| Security Scanning (SonarQube, Trivy & OWASP Dependency Check) | ✔ Completed            |
| Jenkins CI/CD Pipeline Automation                             | ✔ Completed            |
| Docker Hub Image Publishing                                   | ✔ Completed            |
| Monitoring & Observability (Prometheus & Grafana)             | ✔ Completed            |
| Email Notification & Alerting Service                         | ✔ Completed            |
| Amazon EKS Cluster Deployment                                 | ✔ Completed            |
| Argo CD GitOps Implementation                                 | ✔ Completed            |
| Netflix Clone Application Deployment                          | ✔ Successfully Running |

---

# 🎯 Final Result

The complete DevSecOps lifecycle was successfully implemented, covering infrastructure provisioning, security scanning, CI/CD automation, monitoring, alerting, Kubernetes orchestration, and GitOps-based deployment.

The Netflix Clone application is fully deployed on Amazon EKS using industry-standard DevSecOps practices.
<img width="995" height="502" alt="image" src="https://github.com/user-attachments/assets/fe83add3-50f5-46cc-982a-fd3eb189a132" />

---

## ❤️ Why I Built This

I wanted to build a complete real-world DevSecOps project that demonstrates how modern organizations automate software delivery while integrating security, monitoring, and Kubernetes deployment practices into every stage of the development lifecycle.

This project showcases the practical implementation of DevSecOps, GitOps, CI/CD automation, container security, observability, and cloud-native deployment using AWS and Kubernetes.
