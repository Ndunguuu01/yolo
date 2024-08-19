# Week 5 Kubernetes Project

## Overview

This project involves deploying a web application on Google Kubernetes Engine (GKE). The application uses a Docker container and Kubernetes to manage deployment, scaling, and operations. This README provides details about the setup, deployment, and how to access the live application.

## Project Structure

- **Dockerfile**: Defines the image used to run the application.
- **Kubernetes Manifests**: YAML files describing the Kubernetes resources:
  - `Deployment`: Manages stateless application pods.
  - `StatefulSet`: Manages stateful applications with persistent storage.
  - `Service`: Exposes the application to external traffic.
  - `PersistentVolume` and `PersistentVolumeClaim`: Manage storage resources.

## Prerequisites

- **Google Cloud Account**: To set up and manage GKE.
- **Docker Hub Account**: To push and pull Docker images.
- **kubectl**: Kubernetes command-line tool configured to interact with your GKE cluster.
- **gcloud CLI**: Google Cloud SDK to manage your GKE cluster.

## Getting Started

## Deployment

1. **Set up GKE Cluster**: Ensure you have a GKE cluster set up. Follow Google Cloud’s documentation to create and configure your GKE cluster.
2. **Build Docker Image**: Build the Docker image locally and push it to Docker Hub.
    ```bash
    docker build -t ndunguuu/yolo-backend:latest .
    docker push ndunguuu/yolo-backend:latest
    ```
3. **Apply Kubernetes Manifests**: Use the provided YAML files to deploy your application.
    ```bash
    kubectl apply -f manifests/
    ```

4. **Access the Application**: Once deployed, get the external IP of the service to access the application.
    ```bash
    kubectl get services
    ```


