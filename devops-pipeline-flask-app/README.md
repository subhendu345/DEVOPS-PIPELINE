# DevOps Pipeline for Flask App

A complete DevOps project using Flask, Docker, Jenkins, Kubernetes, and Monitoring tools.
# 🚀 DevOps Pipeline for Flask Application

This is a complete DevOps project designed for learning and practice from **Fresher to Advanced Level**. It demonstrates how to containerize a Python Flask application, automate builds and deployments using **Jenkins**, manage infrastructure with **Kubernetes**, and monitor performance using **Prometheus** and **Grafana**.

---

## 📚 Project Highlights

✅ Build a Python Flask microservice  
✅ Dockerize and test the application  
✅ Create a Jenkins CI/CD pipeline  
✅ Deploy to a Kubernetes cluster  
✅ Monitor using Prometheus + Grafana  
✅ Optional Terraform module for cloud infra provisioning  

---

## 🛠 Tech Stack

| Tool            | Purpose                        |
|-----------------|---------------------------------|
| Python + Flask  | Web application (microservice) |
| Docker          | Containerization               |
| Jenkins         | CI/CD Automation               |
| Kubernetes      | Container Orchestration        |
| Prometheus      | Application Monitoring         |
| Grafana         | Dashboard & Metrics            |
| Terraform (opt) | Cloud Infrastructure (IaC)     |

---

## 📁 Folder Structure
devops-pipeline-flask-app/
│
├── app/ # Flask App
│ ├── app.py
│ ├── requirements.txt
│ └── Dockerfile
│
├── jenkins/ # Jenkins Pipeline
│ └── Jenkinsfile
│
├── k8s/ # Kubernetes Deployment
│ ├── deployment.yaml
│ ├── service.yaml
│ └── ingress.yaml (optional)
│
├── monitoring/ # Prometheus + Grafana
│ ├── prometheus.yaml
│ └── grafana-dashboards/
│ └── dashboard.json
│
├── terraform/ (optional) # Cloud Infra Provisioning
│ └── main.tf
│
└── README.md # You're here 😄

---

## ⚙️ Step-by-Step Guide

### 1. 🧱 Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/devops-pipeline-flask-app.git
cd devops-pipeline-flask-app
cd app
pip install -r requirements.txt
python app.py

 🐳 Dockerize Flask App

docker build -t flask-devops:latest ./app
docker run -p 5000:5000 flask-devops:latest

 🔁 Jenkins CI/CD Pipeline

Install Jenkins locally or via Docker.
Set DockerHub credentials as dockerhub-creds.
Use the jenkins/Jenkinsfile in a Jenkins Pipeline job.

Stages:
#1 Clone repo
#2 Build Docker image
#3 Run tests
#4 Push to DockerHub

☸️ Kubernetes Deployment

Apply the Kubernetes manifests:
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml
Access service:
kubectl get svc flask-service

 📊 Monitoring with Prometheus & Grafana

Launch Prometheus with prometheus.yaml.

Import dashboard.json into Grafana.

Monitor Flask app metrics.
**
