<div align="center">

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" width="80" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" width="80" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="80" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="80" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/maven/maven-original.svg" width="80" />
<img src="https://www.vectorlogo.zone/logos/jenkins/jenkins-icon.svg" width="80" />

<br>

### Docker • Docker Compose • Maven • GitHub Actions • Jenkins • CI/CD
![Course](https://img.shields.io/badge/Course-INT332-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![Units](https://img.shields.io/badge/Units-6%2F6-orange?style=for-the-badge)
![Docker](https://img.shields.io/badge/Docker-Containerization-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-CI/CD-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-CI-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-Build_Automation-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)

---

### 👨‍🎓 Academic Information
| Field | Details |
|---------|---------|
| 📘 Course | INT332 – DevOps Virtualization and Configuration Management |
| 🏫 University | Lovely Professional University |
| 🎓 Program | B.Tech Computer Science & Engineering |
| 👨‍💻 Maintained By | Prashant |
| 📂 Repository Type | Notes + Labs + Projects + Viva + Interview Preparation |
| 📈 Coverage | Complete Course Coverage |

</div>

---

# 📖 About This Repository
This repository contains comprehensive notes, practical exercises, commands, projects, viva questions, interview preparation material, and real-world examples covering the complete syllabus of **INT332 – DevOps Virtualization and Configuration Management**.

The content is structured week-by-week and mapped unit-wise to include both theoretical concepts and practical implementations used in modern DevOps environments.

This repository can be used as:

- 📚 Academic Notes
- 💻 Lab Manual
- 🎯 Viva Preparation Guide
- 💼 Interview Preparation Resource
- 🚀 DevOps Learning Roadmap
- 🛠 Practical Reference Guide

---

# 🎯 Course Learning Outcomes
After completing this repository, learners will be able to:

✅ Understand DevOps principles and workflows

✅ Understand virtualization and containerization

✅ Work with Docker and Docker Compose

✅ Create and manage Docker Images

✅ Write optimized Dockerfiles

✅ Manage Docker Networking and Storage

✅ Build Java applications using Maven

✅ Manage dependencies and plugins

✅ Implement Continuous Integration using GitHub Actions

✅ Create automated CI pipelines

✅ Build enterprise-grade CI/CD pipelines using Jenkins

✅ Integrate Docker, Maven, GitHub, and Jenkins

✅ Deploy applications to servers and cloud environments

---

# 🧰 Technology Stack
<div align="center">

| Technology | Purpose |
|------------|----------|
| 🐳 Docker | Containerization |
| 🏗 Docker Compose | Multi-Container Applications |
| ☕ Maven | Build Automation |
| 🌐 Git & GitHub | Version Control |
| ⚡ GitHub Actions | Continuous Integration |
| 🔥 Jenkins | Continuous Delivery & Deployment |
| 🐧 Linux | Container Runtime Environment |
| 📦 Docker Hub | Container Registry |
| 🏢 GitHub Container Registry (GHCR) | Image Registry |
| 🚀 CI/CD | Software Delivery Automation |

</div>

---

# 🛤 Learning Journey
```mermaid
flowchart LR

A[DevOps Fundamentals]
--> B[Containers]

B --> C[Docker]

C --> D[Dockerfile]

D --> E[Docker Compose]

E --> F[Maven]

F --> G[GitHub Actions]

G --> H[Jenkins]

H --> I[CI/CD Pipelines]

I --> J[Production Deployment]
```

---

# 📂 Repository Structure
```text
INT332/
├── week01/                  # Introduction to Containerization & VM Comparisons
├── week02/                  # Docker Basics, CLI Commands & Storage Volumes
├── week03/                  # Mastering 'docker run', flags & environment variables
├── week04/                  # Architecture Evolution (Monolithic vs Microservices)
├── week05/                  # Containers, Docker Compose & Kubernetes Overview
├── week06/                  # Maven Build Tool Fundamentals & Docker Integration
├── week07/                  # Maven + Docker Integration (Practical Labs)
├── week08/                  # Continuous Integration with GitHub Actions
├── week09/                  # Continuous Integration with Jenkins
├── week10_practical/        # Flask + Docker CI pipeline with GitHub Actions
├── week11_practical/        # Production CD Deployment Pipeline
├── week12_practical/        # Java Maven Build & Docker Hub Automation
└── README.md                # Main documentation hub
```

---

## 📚 Unit I – Basics of DevOps Infrastructure
### Topics Covered
#### DevOps Fundamentals
- Introduction to DevOps
- Need for DevOps
- DevOps Lifecycle
- Agile vs DevOps
- Lean vs DevOps

#### Containers & Virtualization
- Evolution of Application Architecture
- Virtual Machines vs Containers
- Container Runtime

#### Linux Internals
- Process Isolation
- Namespaces
- cgroups

#### Docker Fundamentals
- Docker Architecture
- Docker Daemon
- Docker CLI
- Docker Hub

#### Docker Object Types
- Images
- Containers
- Networks
- Volumes

#### Storage & Filesystem
- Docker Layers
- OverlayFS
- Copy-On-Write

#### Practicals & Study Resources
- 📄 [Week 1: Introduction to Containerization](./week01/containerization_guide.md)
- 📄 [Week 2: Docker Basics & CLI Commands](./week02/docker_basics_guide.md)
- 📄 [Week 3: Mastering `docker run` flags](./week03/docker_commands_env_vars.md)

**✅ Unit Status: Complete**

---

## 🐳 Unit II – Image Building & Container Management
### Topics Covered
#### Dockerfile Concepts
- Build Context
- .dockerignore
- Docker Build Process

#### Dockerfile Instructions
- FROM
- RUN
- COPY
- ADD
- CMD
- ENTRYPOINT
- WORKDIR
- ENV
- EXPOSE
- VOLUME

#### Image Management
- Tagging
- Versioning
- Image History
- Layer Inspection

#### Docker Networking
- Bridge Network
- Host Network
- Overlay Network
- DNS
- Port Mapping

#### Docker Storage
- Volumes
- Bind Mounts
- Persistent Data

#### Registries
- Docker Hub
- GHCR
- Private Registries
- Authentication Tokens

#### Practicals & Study Resources
- 📄 [Week 2: Docker Basics & CLI Commands (Networking/Storage/Lab)](./week02/docker_basics_guide.md)
- 📄 [Week 3: Mastering `docker run` flags (Configuration/Env/Registry)](./week03/docker_commands_env_vars.md)
- 📄 [Week 1: Introduction to Containerization (Dockerfile Intro)](./week01/containerization_guide.md)

**✅ Unit Status: Complete**

---

## 🏗 Unit III – Microservices & Docker Compose
### Topics Covered
#### Architecture Evolution
- Monolithic Architecture
- Component-Based Architecture
- Microservices Architecture

#### Docker Compose
- Compose Fundamentals
- YAML Structure
- Services
- Networks
- Volumes
- Environment Variables

#### Commands
- compose up
- compose down
- compose build
- compose logs
- compose restart

#### Practical Examples
- Nginx + MySQL
- Node.js + MongoDB
- Multi-Service Deployments

#### Best Practices
- Compose Design
- Environment Management
- Production Guidelines

#### Practicals & Study Resources
- 📄 [Week 4: Monolithic vs. Microservices Architecture](./week04/monolithic_and_microservices.md)
- 📄 [Week 5: Containers & Docker Compose Orchestration](./week05/containers_and_docker_compose.md)

**✅ Unit Status: Complete**

---

## ☕ Unit IV – Maven Build Automation
### Topics Covered
#### Maven Fundamentals
- Why Build Tools Exist
- Maven Architecture
- Build Automation

#### Project Object Model
- pom.xml
- Dependencies
- Plugins

#### Build Lifecycle
- validate
- compile
- test
- package
- verify
- install
- deploy

#### Dependency Management
- Dependency Scope
- Transitive Dependencies
- Version Conflicts
- Resolution Strategies

#### Maven Plugins
- Compiler Plugin
- Surefire Plugin
- Shade Plugin

#### Maven Wrapper
- mvnw
- Wrapper Benefits

#### Maven + Docker
- Docker Integration
- Dockerized Java Applications

#### Practicals & Study Resources
- 📄 [Week 6: Maven & Build Automation Basics](./week06/maven_and_docker_integration.md)
- 📄 [Week 7: Maven + Docker Practical Integration](./week07/practical_mvn_docker_integration.md)

**✅ Unit Status: Complete**

---

## ⚡ Unit V – Continuous Integration with GitHub Actions
### Topics Covered
#### CI Fundamentals
- Continuous Integration
- Workflow Automation

#### GitHub Actions Components
- Workflows
- Jobs
- Steps
- Actions
- Runners

#### Workflow Triggers
- push
- pull_request
- schedule
- workflow_dispatch

#### Advanced Workflows
- Matrix Builds
- Multi-Job Pipelines
- Caching

#### Runners
- GitHub Hosted Runners
- Self Hosted Runners

#### Docker Integration
- Docker Build
- Docker Hub Push
- GHCR Push

#### Deployment
- Server Deployment
- Cloud Deployment

#### Practicals & Study Resources
- 📄 [Week 8: GitHub Actions CI Workflows](./week08/github_actions_guide.md)
- 📄 [Week 10 (Practical): Flask + Docker CI Pipeline](./week10_practical/flask_docker_github_actions.md)
- 📄 [Week 11 (Practical): Production CD Deployment Pipeline](./week11_practical/actions_deployment_pipeline.md)

**✅ Unit Status: Complete**

---

## 🔥 Unit VI – CI/CD with Jenkins
### Topics Covered
#### Jenkins Foundations
- Introduction to Jenkins
- Architecture
- Controller-Agent Model
- Installation
- Dashboard

#### Security & Administration
- Plugin Management
- User Management
- Credentials
- Security

#### Pipelines
- Freestyle Jobs
- Pipeline Jobs
- Declarative Pipeline
- Scripted Pipeline
- Jenkinsfile

#### Pipeline Stages
- Checkout
- Build
- Test
- Package
- Deploy

#### Docker Integration
- Docker Build
- Docker Agents
- Docker Hub
- GHCR

#### Maven Integration
- Maven Installation
- Build Execution
- Reports
- Coverage

#### GitHub Integration
- Webhooks
- PollSCM
- Multi-Branch Pipelines

#### Deployment
- SSH Agents
- Container Agents
- Cloud Deployment

#### Backup & Recovery
- Jenkins Backup
- Restore Strategies

#### Practicals & Study Resources
- 📄 [Week 9: Jenkins CI/CD Fundamentals](./week09/jenkins_cicd_guide.md)
- 📄 [Week 12 (Practical): Java Maven Build & Docker Hub Automation](./week12_practical/java_maven_docker_hub.md)

**✅ Unit Status: Complete**

---

## 📊 Repository Progress Dashboard
| Unit | Topic | Status |
|--------|--------|---------|
| Unit I | DevOps Infrastructure | ✅ |
| Unit II | Image Building & Container Management | ✅ |
| Unit III | Docker Compose & Microservices | ✅ |
| Unit IV | Maven Build Automation | ✅ |
| Unit V | GitHub Actions (CI) | ✅ |
| Unit VI | Jenkins (CI/CD) | ✅ |

<br>

```text
████████████████████████████████████ 100%
```

---

# 🚀 Practical Coverage
This repository includes:
- [x] Docker Commands
- [x] Dockerfile Projects
- [x] Docker Compose Labs
- [x] Maven Projects
- [x] GitHub Actions Workflows
- [x] Jenkins Pipelines
- [x] Docker Hub Integration
- [x] GitHub Container Registry (GHCR)
- [x] Multi-Container Applications
- [x] End-to-End CI/CD Projects

---

# 🎓 Viva Preparation Included
Topics Covered:
- DevOps Concepts
- Virtualization
- Containers
- Docker Architecture
- Docker Networking
- Docker Storage
- Docker Compose
- Maven Lifecycle
- Maven Plugins
- GitHub Actions
- Jenkins Architecture
- Jenkins Pipelines
- CI/CD Concepts
- Docker Hub
- GHCR

---

# 💼 Interview Preparation Included
Frequently Asked Areas:
- DevOps Lifecycle
- Docker Internals
- Namespaces & cgroups
- Docker Networking
- Docker Storage
- Docker Compose
- Maven Lifecycle
- Dependency Management
- GitHub Actions
- Jenkins Pipelines
- CI/CD Architecture
- Jenkins + Docker
- Jenkins + Maven
- Docker Registries

---

# 🏆 Key Highlights
✨ Complete Unit-wise Notes

✨ Hands-on Labs

✨ Real-World Examples

✨ Docker Projects

✨ Maven Projects

✨ GitHub Actions Workflows

✨ Jenkins CI/CD Pipelines

✨ Viva Questions

✨ Interview Questions

✨ Industry-Oriented Content

---

# 📈 DevOps Roadmap Covered
```text
DevOps
   ↓
Containers
   ↓
Docker
   ↓
Dockerfile
   ↓
Docker Compose
   ↓
Maven
   ↓
GitHub Actions
   ↓
Jenkins
   ↓
CI/CD
   ↓
Production Deployment
```

---

🎓 B.Tech Computer Science & Engineering

🏫 Lovely Professional University

📚 INT332 – DevOps Virtualization and Configuration Management

---

<div align="center">

**Docker • Docker Compose • Maven • GitHub Actions • Jenkins**

If you found this repository useful, consider giving it a ⭐

**Happy Learning & Happy Building! 🚀**

</div>
