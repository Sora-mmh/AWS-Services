# AWS-Services

The listed project in this module cover:

### **1. Jenkins → EC2 Deployment (3 progressive demos)**
- **Part I – Freestyle/SSH push**  
  - Installed Jenkins **SSH Agent plugin**.  
  - Stored **EC2 SSH credentials** in Jenkins.  
  - Pipeline step: `ssh-agent` executes `docker run` on the target EC2 host.  

- **Part II – Docker-Compose push**  
  - Installed **Docker-Compose** on EC2.  
  - Provided `docker-compose.yml` for multi-container stacks.  
  - Jenkins stage runs `docker-compose up -d` via shell.  

- **Part III – Full CI/CD with dynamic versioning**  
  - Extended the Jenkinsfile to **tag images with build numbers**.  
  - Pushed images to **DockerHub** (then to **ECR** (Elastic Container Registry) but the code is not pushed).  
