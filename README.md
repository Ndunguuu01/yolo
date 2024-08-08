# Ecommerce App Configuration Management

## Overview

This challenge demonstrates using Ansible for configuration management to install a containerized e-commerce utility on a Vagrant-provisioned Ubuntu virtual system (VM). The utility is served using Nginx and Docker is used for containerization.

## Project Structure

- **Vagrantfile**: Configuration for provisioning the VM.
- **playbook.Yml**: Ansible playbook for provisioning and configuration.
- **roles/**: Contains Ansible roles for numerous configurations:
  - **frontend/**: Nginx setup.
  - **backend/**: Docker and application setup.
  - **database/**: Database container setup.
- **templates/**:  templates for configuration files.
- **hosts**: Ansible host report.

## Setup Instructions

### Prerequisites

1. **Vagrant**: [Install Vagrant]
2. **VirtualBox**: [Install VirtualBox]

### Provisioning the VM

1. **Clone the Repository**

   ```bash
   git clone https://github.Com/ndunguuu01/yolo.Git
   cd your-repo