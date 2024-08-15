This project has the goal to automate the setup of an e-commerce platform. It uses Ansible, Docker, and Vagrant to achieve this. The process involves creating a virtual machine  with Vagrant setting it up with Ansible, and splitting tasks into roles for the frontend, backend, and database parts.

Vagrant Setup

The project starts by making a specific folder for the files. It initializes Vagrant to create a VM using Ubuntu 20.04. Then, it changes the Vagrantfile to assign resources like memory. The "vagrant up" command brings the VM online and sets it up.

Ansible Setup

The process installs Ansible on the local machine to handle the setup. It creates an organized folder structure to arrange the tasks for different platform components: frontend, backend, and database. An Ansible playbook automates the installation and setup of these components. The frontend role installs and runs Nginx, while the backend role sets up Docker.

Testing the Configuration


The last stage requires connecting to the VM via SSH and executing the Ansible playbook. This action sets up the e-commerce platform making sure all parts are installed and set up.
