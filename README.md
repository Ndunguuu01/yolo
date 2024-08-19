# Kubernetes Deployment Project - Week 5

## Overview

This project showcases the deployment of a web application using Kubernetes on Google Kubernetes Engine (GKE). The application is containerized using Docker and managed using Kubernetes objects such as Deployments, StatefulSets, Services, and PersistentVolumes. The project demonstrates the orchestration of containers and the use of Kubernetes features to ensure scalability, reliability, and persistence.

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

### 1. Clone the Repository

```bash
git clone https://github.com/Ndunguuu01/yolo
cd yolo
