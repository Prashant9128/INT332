# 🚀 INT332: DevOps, Virtualization & Configuration Management
### *Personal Learning Journal & Practical CI/CD Portfolio*

---

## 📋 Workspace Profile
| Identifier | Details |
| :--- | :--- |
| **Student Engineer** | Prashant Kumar Sharma |
| **Institution** | Lovely Professional University |
| **Department** | B.Tech - Computer Science & Engineering |
| **Course Code** | INT332 |
| **Focus Areas** | Virtualization, Container Runtimes, Maven, GitHub Actions, Jenkins |
| **Status** | 12 Weeks of Lectures & Practicals Completed |

---

## 📖 Workspace Overview
This repository serves as my academic logbook and engineering workspace for **INT332**. It contains complete conceptual notes, practical lab execution steps, custom build configurations, and multi-stage pipeline files. 

The workspace is organized chronologically by week, mapping the journey from core operating system isolation primitives up to production-grade deployment pipelines.

---

## 🧰 Technology Matrix & Tooling Stack

```text
  [Runtime & OS]       [Build & Pack]      [CI/CD Pipelines]      [Registries]
 ┌──────────────┐     ┌──────────────┐     ┌───────────────┐     ┌──────────────┐
 │ Linux Kernel │ ──> │ Apache Maven │ ──> │ GitHubActions │ ──> │  Docker Hub  │
 │ Docker Engine│     │ Multi-Stage  │     │ Jenkins (E2E) │     │  GitHub GHCR │
 └──────────────┘     └──────────────┘     └───────────────┘     └──────────────┘
```

* **System Primitives**: Linux Namespaces (PID, NET, MNT, IPC, UTS), control groups (`cgroups`), and OverlayFS.
* **Container Core**: Docker Engine, low-level (`runc`) & high-level (`containerd`) runtimes.
* **Orchestration**: Multi-container service definitions with Docker Compose.
* **Build Automation**: Lifecycle packaging and dependency resolution with Maven.
* **Continuous Integration**: Declarative GitHub Actions workflows and local runners.
* **Continuous Delivery**: Jenkins controller-agent distribution pipelines.

---

## 🗺️ Learning Roadmap
This diagram represents the conceptual pipeline followed throughout the 12-week course:

```mermaid
flowchart TD
    subgraph Phase 1: Container Infrastructure
        W1[Week 1: Containerization Primitives] --> W2[Week 2: Docker CLI & Networking]
        W2 --> W3[Week 3: run Flags & Env Variables]
    end

    subgraph Phase 2: Architecture & Orchestration
        W4[Week 4: Monolithic vs Microservices] --> W5[Week 5: Compose Orchestration]
    end

    subgraph Phase 3: Build Systems
        W6[Week 6: Maven Package Management] --> W7[Week 7: Maven-Docker Integration]
    end

    subgraph Phase 4: CI/CD Workflows
        W8[Week 8: GitHub Actions Core] --> W10[Week 10: Flask Pipeline Lab]
        W10 --> W11[Week 11: CD Server Deployments]
    end

    subgraph Phase 5: Enterprise Pipelines
        W9[Week 9: Jenkins Controller-Agent] --> W12[Week 12: Java Pipeline Automation]
    end

    Phase 1 --> Phase 2 --> Phase 3 --> Phase 4 --> Phase 5
```

---

## 📂 Lab Journal & Weekly Indexes

### 📦 Phase 1: Containerization & CLI Basics (Weeks 1-3)
*Deep dive into virtualization history, Linux container internals, and basic Docker command configurations.*
* 📄 [Week 1: Introduction to Containerization](./week01/containerization_guide.md) — *Hypervisors vs. Containers, Namespaces, Cgroups, Container Runtimes, and Image Layers.*
* 📄 [Week 2: Docker CLI & Storage](./week02/docker_basics_guide.md) — *Lifecycle commands (run, stop, exec), Port Mapping, Volume Mounts, and Apache deployments.*
* 📄 [Week 3: Advanced run Configuration](./week03/docker_commands_env_vars.md) — *Interactive shell execution, environment variable pass-through, and container cleanup flags.*

### 🏛️ Phase 2: Architecture Evolution & Compose Orchestration (Weeks 4-5)
*Focuses on the transition from monoliths to microservices, and orchestrating multi-container environments.*
* 📄 [Week 4: Monolithic vs. Microservices Architecture](./week04/monolithic_and_microservices.md) — *Design paradigms, API communications, scaling characteristics, and benefits/trade-offs.*
* 📄 [Week 5: Docker Compose Orchestration](./week05/containers_and_docker_compose.md) — *Compose YAML files, service link networking, DB volume persistence, and WordPress setup.*

### 🛠️ Phase 3: Build Automation & Package Managers (Weeks 6-7)
*Understanding build tools, package managers, dependency compilation, and dockerizing compiled binaries.*
* 📄 [Week 6: Maven Fundamentals](./week06/maven_and_docker_integration.md) — *POM.xml structure, Maven Build Lifecycle, dependency scope, and custom Java dockerization.*
* 📄 [Week 7: Maven + Docker Lab](./week07/practical_mvn_docker_integration.md) — *Packaging Java code and automated image building with the Maven compiler.*

### 🚀 Phase 4: Continuous Integration with GitHub Actions (Weeks 8, 10, 11)
*Automating code integration, running tests, checking syntax, and deploying to production cloud servers.*
* 📄 [Week 8: GitHub Actions CI Workflows](./week08/github_actions_guide.md) — *Workflows, job runner execution, secrets handling, and registry publishing.*
* 📄 [Week 10: Flask Pipeline Lab](./week10_practical/flask_docker_github_actions.md) — *E2E testing, style checks (flake8), building images, and pushing to Docker Hub.*
* 📄 [Week 11: CD Server Deployment](./week11_practical/actions_deployment_pipeline.md) — *SSH deployments, target key configurations, and live release automation.*

### 🔄 Phase 5: Enterprise Automation with Jenkins (Weeks 9, 12)
*Writing declarative Jenkinsfiles, managing agents, testing Java projects, and publishing artifacts.*
* 📄 [Week 9: Jenkins CI/CD Fundamentals](./week09/jenkins_cicd_guide.md) — *Controller-agent execution, pipeline scripting, Git webhooks, and credential storage.*
* 📄 [Week 12: Java Maven Docker Hub Pipeline](./week12_practical/java_maven_docker_hub.md) — *Complete Jenkinsfile compiling, testing, archiving, building, and publishing Java applications.*

---

## 🎯 Viva & Technical Exam Topics
The following topics are detailed inside the notes and serve as a quick study guide for viva examinations:
1. **Linux Virtualization Internals**:
   * *Namespaces (Isolation)*: PID (Processes), NET (Interfaces), MNT (Filesystem), UTS (Hostname).
   * *cgroups (Limits)*: Allocating max memory, CPU shares, and network bandwidth.
2. **Storage and Filesystem Layers**:
   * *OverlayFS*: Merging lower read-only layers with a top container writable layer.
   * *Copy-on-Write (CoW)*: Modifying image files by copying them to the writable layer on-demand.
3. **Maven Build Lifecycle Phases**:
   * `validate` ➔ `compile` ➔ `test` ➔ `package` ➔ `verify` ➔ `install` ➔ `deploy`.
4. **Declarative Pipelines vs Scripted**:
   * Structural YAML-like Jenkins syntax vs Groovy script flows.

---

## 🏆 Portfolio Highlights & Lab Deliverables
* **Multi-Container Apps**: Implemented Node.js + MongoDB and WordPress + MySQL environments.
* **Optimized Builds**: Built multi-stage Dockerfiles for Java Maven packages to minimize image sizes.
* **Automated CI/CD**: Completed automated Flask testing/packaging via GitHub Actions.
* **Enterprise CI/CD**: Constructed E2E Jenkins pipelines using local runners, credentials keys, and Docker Hub publishes.

---

<div align="center">

**Developed with academic diligence for INT332**  
*If you find these resources helpful, feel free to bookmark/star this repository!*  

**🚀 Code, Automate, & Deploy**

</div>
