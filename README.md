 ISEC6000-SecureDevOps
Secure DevOps Project for ISEC6000 21749180

 Project Overview

Welcome to the ISEC6000 Secure DevOps project repository! This project focuses on the deployment and securing of a microservices-based e-commerce application utilizing Saleor. The setup includes creating a robust Kubernetes environment using Google Kubernetes Engine (GKE), deploying Saleor with Docker Compose, and implementing stringent security measures to safeguard the application.

 Table of Contents

- [Project Overview](project-overview)
- [Setup Instructions](setup-instructions)
- [Task 1: Set Up Initial Infrastructure](task-1-set-up-initial-infrastructure)
- [Task 2: Microservices Architecture and Deployment](task-2-microservices-architecture-and-deployment)
- [Task 3: Implementing Security Measures](task-3-implementing-security-measures)
- [Task 4: Architecture Visualization](task-4-architecture-visualization)
- [References](references)

 Setup Instructions

 Prerequisites

Before starting, ensure you have the following installed and configured:
- Google Cloud SDK: For managing Google Cloud resources.
- kubectl: Command-line tool for interacting with Kubernetes clusters.
- Docker: To manage and deploy containerized applications.
- Git: For version control.
- Trivvy: for vulnerability scanning
  Additional tools like chocolatey to install trivvy for windows

 Installation and Configuration

1. Clone the Repository

   ```bash
   git clone https://github.com/YOUR_USERNAME/ISEC6000-SecureDevOps.git
   cd ISEC6000-SecureDevOps
   ```

2. Set Up the Kubernetes Cluster

   Follow the instructions in [Task 1](task-1-set-up-initial-infrastructure) to create and configure your Kubernetes cluster on GKE.

3. Deploy Saleor

   - Explore the Saleor components and follow the instructions in [Task 2](task-2-microservices-architecture-and-deployment) to deploy the Saleor platform with Docker Compose.
   - Ensure the Saleor Dashboard is accessible at port 9002.

4. Apply Security Measures

   - Refer to [Task 3](task-3-implementing-security-measures) for securing Docker containers and performing vulnerability scans.

5. Review Architecture Visualization

   - Check [Task 4](task-4-architecture-visualization) for the architecture diagram illustrating the service interactions and security measures.

 Task 1: Set Up Initial Infrastructure

 Overview

In this task, the goal was to establish the foundational infrastructure required for the Saleor application. This involved creating a Kubernetes cluster on GKE and setting up version control on GitHub.

 Steps

1. Create a Kubernetes Cluster
   - Provisioned a Kubernetes cluster with the specified settings on Google Kubernetes Engine.

2. Configure kubectl
   - Installed and authenticated `kubectl` to manage the Kubernetes cluster from the local machine.

3. GitHub Repository Setup
   - Created a repository named `ISEC6000-SecureDevOps`.
   - Initialized with a README file and set the repository visibility to Public.

 Task 2: Microservices Architecture and Deployment

 Overview

This task involved deploying the Saleor platform within a Kubernetes environment, customizing Docker Compose files, and ensuring proper service deployment.

 Steps

1. Explore Saleor
   - Investigated the Saleor API, Dashboard, and Platform repositories.
   - Forked the Saleor platform repository to my GitHub account.

2. Customize and Deploy
   - Modified Docker Compose configurations to assign port 9002 to the Saleor Dashboard.
   - Deployed the Saleor stack and verified that all services were operational.

3. Version Control
   - Committed the configuration changes to the forked repository and tagged the commit as `isec6000-assignment1`.


 Task 3: Implementing Security Measures

 Overview

This task focused on securing Docker containers and scanning for vulnerabilities to ensure the application's security.

 Steps

1. Container Security
   - Applied best practices for container security, including non-root user execution and secure base images.

2. Vulnerability Scanning
   - Utilized Trivy to scan for vulnerabilities in container images.
   - Addressed identified issues by updating affected libraries.

 Task 4: Architecture Visualization

 Overview

An architecture diagram was created to visualize the components and their interactions within the Saleor application stack.

 Diagram Details

1. Diagram Components
   - Services: Saleor API, Dashboard, PostgreSQL, Redis.
   - Volumes: Persistent storage for PostgreSQL.
   - Networks: Internal communication paths between services.
   - Ports: Port 9002 for the Saleor Dashboard.

2. Annotations
   - Labeled service interactions and highlighted security aspects such as firewall rules.


 References

1. Saleor Platform Repository. GitHub. [https://github.com/saleor/saleor-platform](https://github.com/saleor/saleor-platform)
2. Saleor API Repository. GitHub. [https://github.com/saleor/saleor](https://github.com/saleor/saleor)
3. Saleor Dashboard Repository. GitHub. [https://github.com/saleor/saleor-dashboard](https://github.com/saleor/saleor-dashboard)
4. Google Cloud Documentation – GKE. [https://cloud.google.com/kubernetes-engine/docs](https://cloud.google.com/kubernetes-engine/docs)
5. Trivy - A Simple and Comprehensive Vulnerability Scanner for Containers. [https://aquasecurity.github.io/trivy](https://aquasecurity.github.io/trivy)
6. Docker Documentation. Best Practices for Writing Dockerfiles. [https://docs.docker.com/develop/develop-images/dockerfile_best-practices](https://docs.docker.com/develop/develop-images/dockerfile_best-practices)
7. Kubernetes Documentation. [https://kubernetes.io/docs](https://kubernetes.io/docs)

---

Feel free to adjust any section as needed for accuracy or personal touch!
