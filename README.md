# Project Overview

This project focuses on implementing continuous delivery for Docker containers, ensuring fast, automated deployment of containers to a Kubernetes cluster. This setup is integral for applications built in a microservices architecture, enabling continuous build, testing, and deployment processes. The automated pipeline accelerates the deployment process as soon as code changes are committed, streamlining operations and reducing dependencies on manual processes.

## Technology Stack and Patterns

### Backend Technologies

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![SonarQube](https://img.shields.io/badge/SonarQube-4E9BCD?style=for-the-badge&logo=sonarqube&logoColor=white)

### CI/CD Tools

![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apache-maven&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white)

### Testing & Security

![Checkstyle](https://img.shields.io/badge/Checkstyle-F7DF1E?style=for-the-badge&logo=java&logoColor=black)
![SonarQube Scanner](https://img.shields.io/badge/SonarQube%20Scanner-4E9BCD?style=for-the-badge&logo=sonarqube&logoColor=white)

### Additional Tools

![OpenJDK](https://img.shields.io/badge/OpenJDK-FFFFFF?style=for-the-badge&logo=openjdk&logoColor=black)
![AWS CLI](https://img.shields.io/badge/AWS%20CLI-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=black)
![Kubectl](https://img.shields.io/badge/Kubectl-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)

![image](https://github.com/user-attachments/assets/e62b573d-ef39-40c0-86ed-06b4f4badb9c)

## Project Architecture

This project follows an automated sequence of deployment events:

1. A developer pushes a code change to GitHub.
2. Jenkins retrieves the code, Dockerfile, Jenkinsfile, and Helm charts.
3. Code quality is tested using Checkstyle and SonarQube Scanner, with results uploaded to SonarQube Server.
4. If all tests pass, Jenkins builds an artifact with Maven.
5. A Docker image is built and, upon passing all checks, pushed to Docker Hub.
6. Jenkins deploys Helm charts to the Kubernetes cluster, creating resources like pods, services, and volumes.
7. If updates are made, such as a new image tag, changes are applied automatically.

## Key Features

- **Automated CI/CD Pipeline**: Efficient code integration, testing, and deployment from Jenkins to Kubernetes.
- **Version Control and Artifact Management**: Automated versioning and management of Docker images via Jenkins.
- **Real-Time Code Analysis and Testing**: Ensures high code quality with Checkstyle and SonarQube integration.
- **Flexible Deployment Configuration**: Helm charts and kOps enable scalable and flexible deployments.

## My Contribution

In this project, I focused on the complete setup of the CI/CD pipeline, integrating Docker containerization and automated deployment to Kubernetes with Jenkins. My work covered automation scripts for Docker and Kubernetes, configuration of the deployment environment, and the setup of various testing and security tools to streamline code validation and deployment. This hands-on approach provided a robust system for continuous delivery, reducing deployment time and manual dependencies. 
