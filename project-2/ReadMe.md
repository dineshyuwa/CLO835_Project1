# Project Name

## Overview
This project aims to containerize a Python application using Docker and deploy it to Kubernetes. The application displays the current time in Toronto/Canada.

## Prerequisites
- Docker installed locally
- Access to a Kubernetes cluster

## Fork and Clone the Repository
1. **Fork the Repository**: 
   - Fork the repository from [GitHub Repository URL](https://github.com/sojoudian/clo835_s24).
   
2. **Clone the Repository**: 
   ```bash
   git clone https://github.com/your-username/clo835_s24.git

3. **Create a Dockerfile in the root directory of your project**

4. **Build Docker Image**:
docker build -t your-dockerhub-username/app-name:tag .

5. **Push Docker Image**:
docker push your-dockerhub-username/app-name:tag

6. **Create Kubernetes Deployment and Service YAML files.**

7. **minikube start.**

8. **Apply the Kubernetes manifests to deploy your application:**
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

9. **get minikube ip**:
minikubeip

10. **access the application using** :
http://node-ip:32000