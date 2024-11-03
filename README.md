## Fully Automated CI/CD Pipeline with Ansible, Jenkins, and Tomcat Deployment!
This project demonstrates a comprehensive CI/CD pipeline that integrates Ansible with Jenkins to automate the build, test, and deployment of an application across multiple environments, with a focus on Tomcat and Apache setup.

## Project Overview
### Automate Infrastructure Setup:
Using Jenkins and Ansible, the pipeline sets up Tomcat on worker nodes and configures Apache to serve the application.

## Streamline CI/CD Processes:
Jenkins Pipeline automates the entire application lifecycle, from code integration to production deployment.

## Parameterized Deployment:
The pipeline is parameterized to support dynamic deployments across dev and test environments.

## Ensure Consistency:
Ansible manages configurations and deployment tasks across dev, test, and prod environments, ensuring consistent results.

## Key Features
## Tomcat Setup on Worker Nodes:
Automated setup of Tomcat using Ansible [tomcat installation](https://github.com/MASTHAN55/all-setup/blob/main/tomcat.sh) [check version updates befor installation].

## Jenkins & Ansible Integration:
Smooth integration for automated deployments [jenkins-pipeline](https://github.com/MASTHAN55/project-3/blob/main/pipeline).
## Parameterized Pipeline:
AWS CodePipeline is configured with parameterized values for flexibility across dev and test environments. [jenkins-pipeline](https://github.com/MASTHAN55/project-3/blob/main/pipeline)
## Apache Integration:
Automated configuration of Apache web server using Ansible.[deploy-file](https://github.com/MASTHAN55/project-3/blob/main/deploy.yml)
