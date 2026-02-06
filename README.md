# 🚀 FullStack Blogging App – DevOps CI/CD Project

A full-stack blogging application built with **Java (Spring Boot)** and deployed on **AWS EKS** using a complete **DevOps CI/CD pipeline**.  
This project demonstrates real-world DevOps practices including CI/CD, containerization, security scanning, Kubernetes deployment, and monitoring.

---

## 🧠 Project Overview

This project focuses on end-to-end automation:

- Source code management with GitHub  
- Continuous Integration with Jenkins  
- Code quality & security checks  
- Docker image build & push  
- Kubernetes deployment on AWS EKS  
- Monitoring using Prometheus & Blackbox Exporter  
- Email notifications on pipeline completion  

---

## 🛠 Tech Stack

### Application
- Java 17  
- Spring Boot  
- Maven  

### DevOps & Cloud
- Jenkins – CI/CD pipeline  
- Docker – Containerization  
- Docker Hub – Image registry  
- Kubernetes (EKS) – Container orchestration  
- Terraform – Infrastructure provisioning  
- AWS – Cloud provider  

### Security & Quality
- SonarQube – Code quality analysis  
- Trivy – File system & image vulnerability scanning  

### Monitoring
- Prometheus  
- Blackbox Exporter  

---

## ⚙️ CI/CD Pipeline Stages

1. Git Checkout  
2. Maven Compile  
3. Unit Tests  
4. Trivy File System Scan  
5. SonarQube Analysis  
6. Build & Package Application  
7. Publish Artifacts  
8. Docker Build & Tag  
9. Trivy Image Scan  
10. Docker Image Push  
11. Kubernetes Deployment (EKS)  
12. Deployment Verification  
13. Email Notification  

---

## 🐳 Docker Image

Docker image pushed to Docker Hub:

subhadeep2001/blogging_app:latest

---

## ☸️ Kubernetes Deployment

- Namespace: webapps  
- Deployment: bloggingapp-deployment  
- Service Type: LoadBalancer  
- Image pulled using Docker registry secret (regcred)

Application is accessible via the AWS LoadBalancer DNS.

---

## 📊 Monitoring

- Prometheus scrapes application metrics  
- Blackbox Exporter monitors HTTP endpoints and external services  

---

## 📧 Email Notifications

- Jenkins sends HTML email notifications after each pipeline run  
- Includes job name, build number, pipeline status, and console output link  

---

## 🧪 Security Scanning

- Trivy FS Scan – source code scanning  
- Trivy Image Scan – Docker image scanning  
- SonarQube – bug, vulnerability, and code smell detection  

---

## 📂 Repository Structure

.
├── src/  
├── Dockerfile  
├── pom.xml  
├── Jenkinsfile  
├── deployment-service.yml  
├── README.md  

---

## 🚀 How to Run Locally

mvn clean package  
docker build -t blogging_app .  
docker run -p 8080:8080 blogging_app  

Access: http://localhost:8080

---

## 🎯 Key Learnings

- Real-world Jenkins CI/CD pipelines  
- Kubernetes production deployment  
- Secure image handling  
- Infrastructure as Code (Terraform)  
- Monitoring and observability  
- Debugging real DevOps issues  

---

## 👨‍💻 Author
Subhadeep Ghosh  
DevOps | Cloud | Kubernetes | CI/CD

Subhadeep Ghosh  
DevOps | Cloud | Kubernetes | CI/CD
