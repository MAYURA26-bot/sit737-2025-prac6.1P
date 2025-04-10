# SIT737 Task 6.1P – Kubernetes Deployment

This project demonstrates how to deploy a containerized Node.js calculator microservice to a Kubernetes cluster using Docker Desktop with Kubernetes enabled.


##  Application Overview

A simple calculator microservice built with Node.js, containerized using Docker, and deployed using Kubernetes.

##  Prerequisites

- Docker Desktop (with Kubernetes enabled)
- Docker Hub account
- `kubectl` CLI (included with Docker Desktop)

##  Deployment Steps

###  1. Enable Kubernetes in Docker Desktop

1. Open Docker Desktop
2. Go to Settings > Kubernetes
3. Check "Enable Kubernetes"
4. Click **Apply & Restart**

Wait until Kubernetes is running (green status indicator).

### 2. Build and Push Docker Image

1. docker build -t your-dockerhub-username/image-name .
2. docker login
3. docker push your-dockerhub-username/image-name

### 3. Apply Kubernetes Deployment and Service

1. kubectl apply -f deployment.yaml
2. kubectl apply -f service.yaml

### 4. Access the application via the browser

http://localhost:30007

