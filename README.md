# Yolo Project

## Overview

The Yolo Project is a comprehensive application designed to be deployed on Kubernetes. This project includes a Node.js backend service with a Docker container, Kubernetes configurations for deployment, service, and scaling, and various related resources to ensure a robust and scalable application.

## Features

- **Node.js Backend**: A simple Node.js application to serve as the backend service.
- **Docker**: Containerized application using Docker.
- **Kubernetes**: Deployment, service, ingress, and scaling configurations for managing and accessing the application in a Kubernetes cluster.
- **Persistence**: Configurations for Persistent Volumes and Persistent Volume Claims.

## Getting Started

### Prerequisites

- Docker: Ensure Docker is installed and running on your machine.
- Kubernetes: Minikube or a Kubernetes cluster setup.
- kubectl: Kubernetes command-line tool.

### Setup and Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/Ndunguuu01/yolo
   cd yolo-project
2. **Build and Run the Docker Container**


docker build -t ndunguuu/yolo-backend:latest .
docker run -p 8080:8080 ndunguuu/yolo-backend:latest
3.  **Deploy to Kubernetes**

:Apply Kubernetes configurations:

kubectl apply -f k8s/
:Check the status of your pods:


kubectl get pods
:Get the external IP of the service:
kubectl get svc



Testing and Validation


Ensure the Docker container runs properly before deploying to Kubernetes.
Use kubectl to ensure all components are running as expected and validate the deployment.