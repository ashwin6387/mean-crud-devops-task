# 🚀 MEAN Stack DevOps Deployment Project

## 📌 Internship Submission -- DevOps / Cloud Role

This project demonstrates a production-style deployment of a full-stack
**MEAN (MongoDB, Express, Angular, Node.js)** application using modern
DevOps practices.

It showcases:

-   Docker containerization
-   Multi-stage builds
-   Nginx reverse proxy configuration
-   Docker Compose orchestration
-   CI/CD using GitHub Actions
-   Deployment on Ubuntu (AWS EC2 compatible)

------------------------------------------------------------------------

# 🏗 Project Architecture

User → Nginx (Port 80) → Angular Frontend → Node.js Backend → MongoDB

------------------------------------------------------------------------

# 🛠 Technologies Used

-   Angular
-   Node.js + Express
-   MongoDB
-   Docker
-   Docker Compose
-   Nginx
-   GitHub Actions
-   Ubuntu Server (AWS EC2)

------------------------------------------------------------------------

# 📂 Project Structure

mean-crud-devops-task/ │ ├── backend/ │ └── Dockerfile │ ├── frontend/ │
└── Dockerfile │ ├── nginx.conf ├── docker-compose.yml └──
.github/workflows/deploy.yml

------------------------------------------------------------------------

# 🐳 Step 1: Clone Repository

git clone
https://github.com/`<your-username>`{=html}/mean-crud-devops-task.git cd
mean-crud-devops-task

------------------------------------------------------------------------

# ☁️ Step 2: Deployment on Ubuntu Server (AWS EC2)

1.  Launch Ubuntu 22.04 instance
2.  Open port 80 in Security Group
3.  SSH into server

Install Docker:

sudo apt update sudo apt install docker.io docker-compose -y sudo
systemctl enable docker

Clone project:

git clone
https://github.com/`<your-username>`{=html}/mean-crud-devops-task.git cd
mean-crud-devops-task

Run:

docker-compose up -d --build

Access via:

http://`<EC2-PUBLIC-IP>`{=html}

------------------------------------------------------------------------

# 🔄 CI/CD Pipeline (GitHub Actions)

Workflow triggers on push to main branch.

Pipeline performs:

-   Docker Hub login
-   Build backend image
-   Build frontend image
-   Push images to Docker Hub

------------------------------------------------------------------------

# 🔐 Required GitHub Secrets

Add under Repository → Settings → Secrets → Actions

-   DOCKER_USERNAME
-   DOCKER_PASSWORD (Use Docker Hub Access Token)

------------------------------------------------------------------------

# 📊 DevOps Practices Implemented

-   Containerized Microservices Architecture
-   Environment Isolation via Docker
-   Reverse Proxy Configuration
-   Automated Image Build & Push
-   Production-style VM Deployment
-   Clean Code Structure

------------------------------------------------------------------------

# 🎯 Learning Outcomes

Through this project, I gained hands-on experience in:

-   Docker image creation & optimization
-   Service orchestration with Docker Compose
-   CI/CD automation
-   Cloud VM deployment
-   Production-ready reverse proxy setup

------------------------------------------------------------------------

# ✅ Conclusion

This project demonstrates real-world DevOps workflow from development to
deployment using industry-standard tools.

It reflects practical understanding of containerization, CI/CD, and
cloud deployment suitable for an internship-level DevOps/Cloud Engineer
role.
