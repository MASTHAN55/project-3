# Fully Automated CI/CD Pipeline with Ansible, Jenkins, and Tomcat Deployment!
This project demonstrates a comprehensive CI/CD pipeline that integrates Ansible with Jenkins to automate the build, test, and deployment of an application across multiple environments, with a focus on Tomcat and Apache setup.

### Project Overview
### Automate Infrastructure Setup:
Using Jenkins and Ansible, the pipeline sets up Tomcat on worker nodes and configures Apache to serve the application.

### Streamline CI/CD Processes:
Jenkins Pipeline automates the entire application lifecycle, from code integration to production deployment.

### Parameterized Deployment:
The pipeline is parameterized to support dynamic deployments across dev and test environments.
### Ensure Consistency:
Ansible manages configurations and deployment tasks across dev, test, and prod environments, ensuring consistent results.
## Key Features
### Tomcat Setup on Worker Nodes:
Automated setup of Tomcat using Ansible [tomcat installation](https://github.com/MASTHAN55/all-setup/blob/main/tomcat.sh) [check version updates befor installation].
### Jenkins & Ansible Integration:
Smooth integration for automated deployments [jenkins-pipeline](https://github.com/MASTHAN55/project-3/blob/main/pipeline).
### Parameterized Pipeline:
AWS CodePipeline is configured with parameterized values for flexibility across dev and test environments. [jenkins-pipeline](https://github.com/MASTHAN55/project-3/blob/main/pipeline)
### Apache Integration:
Automated configuration of Apache web server using Ansible.[deploy-file](https://github.com/MASTHAN55/project-3/blob/main/deploy.yml)

## How It Works
### Code Integration:
The pipeline triggers whenever a developer pushes code to the GitHub repository.

### Build & Test:
The latest code changes are automatically built and tested.

### Deployment:
Successfully tested builds are deployed to the dev, test, and prod environments using Ansible.

### Getting Started
Jenkins installed and configured 

[jenkins](https://github.com/MASTHAN55/project-3/blob/main/jenkins.sh).


## Ansible installed and configured
 amazon-linux-extras install ansible2 -y

 yum install python3 python-pip python-devel -y

vim /etc/ansible/hosts
Ex 1: Ungrouped hosts, specify before any group headers.

### [dev] 
172.31.20.40   
172.31.21.25

### [test] 
172.31.31.77   
172.31.22.114

ssh-keygen            -- > enter 4 times 
ssh-copy-id root@    private ip of dev-1
## To check worker node connection with ansible server.
 ansible -m ping all 
[worker nodes ping](https://github.com/MASTHAN55/project-3/blob/main/screen-shots/ping%20(2).png)

## Tomcat Setup on Worker Nodes:
Automated setup of Tomcat using Ansible. [Tomcat installtion](https://github.com/MASTHAN55/project-3/blob/main/tomcat.yml)

installation

## Jenkins & Ansible Integration:
Smooth integration for automated deployments.[pipeline](https://github.com/MASTHAN55/project-3/blob/main/pipeline)

## Parameterized Pipeline:
AWS CodePipeline is configured with parameterized values for flexibility across dev and test environments.

## application deployment on worker nodes
[worker node1](https://github.com/MASTHAN55/project-3/blob/main/screen-shots/slave1.png).

[worker node2](https://github.com/MASTHAN55/project-3/blob/main/screen-shots/slave2.png)
