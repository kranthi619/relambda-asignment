# relambda-asiignment
# Three-Tier Web Application Automation

## Overview
This project automates the deployment and configuration of a three-tier web application infrastructure using Vagrant and Ansible. The infrastructure includes Nginx, HAProxy, and MySQL as the three tiers.

## Prerequisites
- Vagrant installed on your machine.
- Ansible installed on your machine.
- Either the Ubuntu Trusty64 or CentOS 6.5 x64 Vagrant boxes.

## Directory Structure
/three-tier-web-app
|-- Vagrantfile
|-- ansible/
| |-- playbook.yml
| |-- roles/
| |-- nginx/
| |-- tasks/
| |-- main.yml
| |-- templates/
| |-- nginx.conf.j2
| |-- haproxy/
| |-- tasks/
| |-- main.yml
| |-- templates/
| |-- haproxy.cfg.j2
| |-- mysql/
| |-- tasks/
| |-- main.yml
| |-- templates/
| |-- my.cnf.j2
|-- README.md


## Step-by-Step Guide
 Clone the Repository
git clone https://github.com/kranthi619/relambda-asignment.git
cd three-tier-web-app


1. Update Vagrantfile
Open Vagrantfile and customize the VM configurations

2.Run Vagrant to Create VMs
  $vagrant up

3.Run Ansible Playbook
  $ansible-playbook -i vagrant_ansible_inventory ansible/playbook.yml

4.Accessing the VMs
 $vagrant ssh VM

5.Customizing Configurations
Customize Nginx configurations in ansible/roles/nginx/templates/nginx.conf.j2.
Customize HAProxy configurations in ansible/roles/haproxy/templates/haproxy.cfg.j2.
Customize MySQL configurations in ansible/roles/mysql/templates/my.cnf.j2.

6.Restart Services
  $vagrant provision

  ## Overview
This project demonstrates my ability to automate the deployment and configuration of a three-tier web application infrastructure using Vagrant and Ansible. The infrastructure consists of Nginx, HAProxy, and MySQL, orchestrated across three VMs.

## Key Steps and Achievements
1. **Infrastructure Setup:**
   - Utilized Vagrant to provision three VMs, each running either Ubuntu Trusty64 or CentOS 6.5 x64.
   - Defined VM configurations in the Vagrantfile.

2. **Automation with Ansible:**
   - Implemented an Ansible playbook (`playbook.yml`) to automate the setup of the entire infrastructure.
   - Created Ansible roles for Nginx, HAProxy, and MySQL, each with specific tasks and configurations.

3. **Configurability:**
   - Templated configurations for Nginx, HAProxy, and MySQL, allowing for easy customization based on specific application requirements.
   - Provided clear instructions in the README.md on how to customize and update configurations.

4. **User-Friendly Instructions:**
   - Wrote a detailed step-by-step guide in the README.md for users to clone the repository, run Vagrant to create VMs, execute the Ansible playbook, and access the VMs.
   - Emphasized the importance of testing the infrastructure and restarting services after configuration updates.

     I appreciate the opportunity to present this project to Relambda and am open to any feedback or discussions regarding the choices made during the implementation.

Thank you for considering my submission.!!!!!!

  
