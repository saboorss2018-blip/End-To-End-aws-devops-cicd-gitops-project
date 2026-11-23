🚀 End-to-End AWS DevOps CI/CD & GitOps Project

📌 Project Overview

This project demonstrates an end-to-end CI/CD pipeline using AWS and DevOps tools.

The application is built using FastAPI and deployed on Amazon EKS using Docker, Jenkins, AWS ECR, Kubernetes, and Argo CD.

🏗️ Project Architecture

```text
Developer
    |
    v
 GitHub
    |
    v
GitHub Webhook
    |
    v
 Jenkins
    |
    v
 SonarQube
    |
    v
 Docker Build
    |
    v
  AWS ECR
    |
    v
 Amazon EKS
    |
    v
 Kubernetes
    |
    v
  Argo CD
    |
    v
 AWS LoadBalancer
    |
    v
 Live Application
```

🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| AWS EC2 | Server Hosting |
| Git & GitHub | Source Code Management |
| GitHub Webhook | Automatic Pipeline Trigger |
| Jenkins | CI/CD Automation |
| SonarQube | Code Quality Analysis |
| Docker | Containerization |
| AWS ECR | Docker Image Storage |
| Amazon EKS | Kubernetes Cluster |
| Kubernetes | Container Orchestration |
| Argo CD | GitOps Deployment |
| AWS LoadBalancer | Application Access |
| Python FastAPI | Application Development |

⚙️ Project Workflow

1. Developer pushes code to GitHub.
2. GitHub Webhook triggers Jenkins automatically.
3. Jenkins pulls the latest source code.
4. SonarQube performs code quality analysis.
5. Jenkins builds the Docker image.
6. Docker image is pushed to AWS ECR.
7. Kubernetes manifests are maintained in GitHub.
8. Argo CD synchronizes the manifests with Amazon EKS.
9. Kubernetes manages application Pods.
10. AWS LoadBalancer exposes the application.

📂 Project Structure

```text
end-to-end-aws-devops-cicd-project/
│
├── README.md
│
├── Source-Code/
│   ├── Dockerfile
│   ├── Jenkinsfile
│   ├── main.py
│   ├── form.html
│   └── requirements.txt
│
└── Deployment-Repo/
    └── k8s/
        └── deployment.yaml
```

🔄 GitHub Webhook Integration

Configured GitHub Webhook to trigger the Jenkins pipeline automatically whenever new code is pushed to the repository.

☸️ Kubernetes Deployment

- Created an Amazon EKS cluster.
- Configured worker nodes.
- Deployed the application using Kubernetes Deployment.
- Configured three replicas.
- Exposed the application using AWS LoadBalancer.
- Configured rolling update strategy.

🔁 Argo CD GitOps

- Installed Argo CD on Amazon EKS.
- Connected Argo CD with GitHub.
- Configured application synchronization.
- Monitored application health and deployment status.

🎯 Key Learnings

- CI/CD Pipeline Automation
- GitHub Webhook Integration
- Docker Image Management
- AWS ECR and EKS
- Kubernetes Deployment
- Argo CD GitOps
- Troubleshooting Pod Scheduling Issues
- Rolling Update Strategies

👨‍💻 Author

Abdul Saboor

Aspiring AWS DevOps Engineer

Skills: AWS | Linux | Jenkins | Docker | Kubernetes | Terraform | Git | GitHub | SonarQube | Argo CD

