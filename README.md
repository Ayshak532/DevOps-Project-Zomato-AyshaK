# 🚀 Zomato Clone – End-to-End DevOps Project

An end-to-end DevOps project demonstrating CI/CD automation, code quality analysis, security scanning, containerization, Kubernetes deployment, GitOps, and monitoring for a Zomato clone application.

## 🧰 Technologies & Tools

![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![SonarQube](https://img.shields.io/badge/SonarQube-4E9BCD?style=flat-square&logo=sonarqube&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP_Dependency--Check-000000?style=flat-square&logo=owasp&logoColor=white)
![Trivy](https://img.shields.io/badge/Trivy-1904DA?style=flat-square)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Argo CD](https://img.shields.io/badge/Argo_CD-EF7B4D?style=flat-square&logo=argo&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Docker Hub](https://img.shields.io/badge/Docker_Hub-2496ED?style=flat-square&logo=docker&logoColor=white)

## 🏗️ Project Architecture

**Source Code → Jenkins CI/CD → SonarQube → OWASP Dependency-Check → Trivy → Docker Build → Docker Hub → Kubernetes → Argo CD → Prometheus → Grafana**

The workflow covers application source management, automated build and analysis, security scanning, container image publishing, Kubernetes deployment, GitOps-based synchronization, and monitoring.

## 🔄 Implementation Stages

### Stage 1: CI/CD and Docker Deployment

- Hosted the application source code in GitHub.
- Configured a Jenkins pipeline for automated build and deployment tasks.
- Integrated SonarQube for static code quality analysis.
- Used OWASP Dependency-Check to identify vulnerable dependencies.
- Used Trivy for filesystem vulnerability scanning.
- Built a Docker image for the application.
- Published the image to Docker Hub.
- Prepared the application for container-based deployment.

### Stage 2: Kubernetes, GitOps and Monitoring

- Configured Kubernetes deployment and service resources.
- Deployed the application using a container image.
- Integrated Argo CD for GitOps-based deployment synchronization.
- Configured Prometheus for metrics collection.
- Used Grafana for monitoring dashboards and visualization.

## 🔗 Project Links

- **GitHub Repository:** [DevOps Project – Zomato](https://github.com/Ayshak532/DevOps-Project-Zomato-AyshaK)
- **Docker Hub Image:** [ayshak/zomato](https://hub.docker.com/r/ayshak/zomato)
- **LinkedIn Profile:** [Aysha K](https://www.linkedin.com/in/aysha-k-b933b5290/)

## 🛠️ Setup Overview

The following is a high-level outline. Adapt the commands and configuration to the files and environment in this repository.

### 1. Clone the repository

```bash
git clone https://github.com/Ayshak532/DevOps-Project-Zomato-AyshaK.git
cd DevOps-Project-Zomato-AyshaK
```

### 2. Build the Docker image

```bash
docker build -t zomato .
```

### 3. Run the container locally

```bash
docker run --name zomato-app -p 3000:3000 zomato
```

Confirm the application's configured port before running the container. Change `3000:3000` if the Dockerfile or application uses a different port.

### 4. Push the image to Docker Hub

After authenticating with Docker Hub and tagging the image:

```bash
docker tag zomato:latest ayshak/zomato:latest
docker push ayshak/zomato:latest
```

### 5. Deploy to Kubernetes

Apply the Kubernetes manifest files from the repository after verifying the image name, namespace, and cluster context.

```bash
kubectl apply -f Kubernetes/
kubectl get deployments,services,pods
```

Check the actual manifest paths and filenames in the repository before running these commands.

## 🎯 Project Objectives

This project provides hands-on practice with:

- CI/CD pipeline automation using Jenkins
- Static code analysis with SonarQube
- Dependency and filesystem vulnerability scanning
- Docker image creation and publishing
- Kubernetes application deployment
- GitOps workflows with Argo CD
- Metrics collection with Prometheus
- Monitoring dashboards with Grafana
- Integrating security checks into a DevOps workflow

## 📚 Learning Reference

This project was developed as a hands-on learning implementation with reference to the following tutorial:

[DevOps Real-time Project – Deployment of Zomato App in Kubernetes Cluster](https://youtu.be/GyoI6-I68aQ)

Credit to the original tutorial creator for the learning reference. The repository reflects my project setup and implementation work. Please refer to the original source and any applicable license terms for reused code or assets.

## 👩‍💻 About Me

I am an **AWS Cloud & DevOps Engineer** interested in cloud infrastructure, CI/CD automation, containerization, Kubernetes, DevSecOps, and monitoring.

- **GitHub:** [Ayshak532](https://github.com/Ayshak532)
- **LinkedIn:** [Aysha K](https://www.linkedin.com/in/aysha-k-b933b5290/)

## 💬 Feedback

I welcome constructive feedback and suggestions to improve this project and my practical DevOps skills.

---

**Thanks for visiting my repository!** 🚀
