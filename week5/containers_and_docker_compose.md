# 🚢 Week 5: Containers, Docker, and Kubernetes

Welcome to **Week 5**! This module bridges the gap between Microservices and actual deployment using **Containers** and orchestration tools like **Docker Compose** and **Kubernetes**.

---

## 📑 Table of Contents
1. [Containers Deep Dive](#1-containers-deep-dive)
2. [Docker & Kubernetes Overview](#2-docker--kubernetes-overview)
3. [Docker Compose Magic](#3-docker-compose-magic)
4. [docker-compose.yml Structure & Concepts](#4-docker-composeyml-structure--concepts)
5. [How Docker Compose Works & Commands](#5-how-docker-compose-works--commands)
6. [Practical Real-World Examples](#6-practical-real-world-examples)
7. [🎓 Interview Prep & Revision](#7-interview-prep--revision)

---

## 1. 📦 Containers Deep Dive

### Definition
Containers are lightweight virtualization technology used to run isolated applications on the same operating system.

### ✨ Features of Containers
* **Lightweight:** Faster than VMs
* **Portable:** Run anywhere
* **Isolated:** Applications separated securely
* **Efficient:** Better resource utilization

### Containers vs Virtual Machines

![Containers vs Virtual Machines](./images/containers_vs_vms.png)

| Feature | Containers | Virtual Machines |
| :--- | :--- | :--- |
| **OS** | Shared Kernel | Separate OS |
| **Speed** | Fast | Slower |
| **Resource Usage** | Low | High |
| **Boot Time** | Seconds | Minutes |

### Containers and Microservices
Microservices usually run inside containers.
* **Why?** Faster deployment, better scalability, isolation, reliability.

---

## 2. 🐳 Docker & Kubernetes Overview

### Docker
**Definition:** Docker is a platform used to create and manage containers.

### Kubernetes (K8s)
**Definition:** Kubernetes is a container orchestration platform.
**Functions:** Auto scaling, Self healing, Load balancing, Container management.

---

## 3. 🪄 Docker Compose Magic

### Definition
Docker Compose is a tool used to manage multi-container Docker applications using a `YAML` file.

### Why Docker Compose is Needed?
Without Compose, you run multiple commands manually:
```bash
docker run web
docker run db
docker run redis
```
> [!WARNING]
> **Problems without Compose:** Too many commands, networking issues, hard configuration, difficult reproducibility.

### 🌟 Benefits of Docker Compose
1. **Multi-container Management:** Manage all containers together.
2. **Reproducibility:** Same setup on every machine.
3. **Simplified Networking:** Services communicate using names.
4. **Dependency Management:** Controls startup order.
5. **Scalability:** Easy scaling using commands.

---

## 4. 📝 docker-compose.yml Structure & Concepts

### Basic Structure
```yaml
version: "3.9"

services:
  web:
    image: nginx
```

### 🧩 Important Concepts

**A. Services:** Blueprint for containers.
**B. Image vs Build:**
* `image: nginx` (Uses existing image)
* `build: .` (Builds custom image)

**C. Ports:** Format is `HostPort : ContainerPort`
```yaml
ports:
  - "8080:80"
```

**D. Volumes:** Used for persistent storage.
```yaml
volumes:
  - data:/var/lib/mysql
```

> [!NOTE]
> **E. Networks:** Compose automatically creates networks for service discovery and built-in DNS.

**F. depends_on:**
```yaml
depends_on:
  - db
```
> [!CAUTION]
> *Important:* `depends_on` ensures startup order, but does **NOT** ensure service readiness.

---

## 5. ⚙️ How Docker Compose Works & Commands

### Workflow
Docker Compose: Reads YAML file ➔ Pulls/Builds images ➔ Creates networks ➔ Creates volumes ➔ Starts containers ➔ Connects services.

### ⌨️ Basic Commands
* **Setup:** `docker-compose version`, `docker-compose config`
* **Starting:** `docker-compose up`, `docker-compose up -d` (detached), `docker-compose up --build`
* **Stopping:** `docker-compose down`, `docker-compose stop`, `docker-compose start`
* **Monitoring:** `docker-compose ps`, `docker-compose logs`, `docker-compose logs -f`
* **Execute Inside:** `docker-compose exec web bash`
* **Scaling:** `docker-compose up --scale web=3`

---

## 6. 🌐 Practical Real-World Examples

### Node.js + MongoDB Example
```yaml
version: '3.8'

services:
  app:
    image: node:18
    container_name: node-app
    working_dir: /usr/src/app
    volumes:
      - .:/usr/src/app
    command: npm start
    ports:
      - "3000:3000"
    environment:
      - MONGO_URL=mongodb://mongo:27017/mydb
    depends_on:
      - mongo

  mongo:
    image: mongo:6
    container_name: mongo-db
    ports:
      - "27017:27017"
    volumes:
      - mongo-data:/data/db

volumes:
  mongo-data:
```

### WordPress + MySQL Example
```yaml
version: '3.8'

services:
  wordpress:
    image: wordpress:latest
    container_name: wordpress-app
    ports:
      - "8080:80"
    environment:
      WORDPRESS_DB_HOST: db:3306
      WORDPRESS_DB_USER: wpuser
      WORDPRESS_DB_PASSWORD: wppass
      WORDPRESS_DB_NAME: wpdb
    depends_on:
      - db

  db:
    image: mysql:5.7
    container_name: mysql-db
    restart: always
    environment:
      MYSQL_DATABASE: wpdb
      MYSQL_USER: wpuser
      MYSQL_PASSWORD: wppass
      MYSQL_ROOT_PASSWORD: rootpass
    volumes:
      - db-data:/var/lib/mysql

volumes:
  db-data:
```

---

## 7. 🎓 Interview Prep & Revision

### Real-World Examples
| Platform | Architecture |
| :--- | :--- |
| WordPress Site | Containerized App |

### 🚀 One-Line Revision Notes
* **Docker** = Container platform
* **Kubernetes** = Container manager
* **Docker Compose** = Multi-container manager
* **Volume** = Persistent storage
* **Port Mapping** = HostPort:ContainerPort
* **YAML** = Indentation-sensitive configuration format

### 📝 Important Interview / Viva Questions
**Q2. Why are containers faster than VMs?**
* Because containers share the host OS kernel.

**Q3. What is Docker Compose?**
* Tool for managing multiple containers using YAML configuration.

**Q4. What is Kubernetes?**
* Container orchestration platform for scaling and managing containers.

**Q5. What is the purpose of depends_on?**
* Controls startup order of services.

> [!IMPORTANT]
> **Important Keywords:**
> `Containers`, `Docker`, `Kubernetes`, `Docker Compose`, `YAML`, `Volumes`, `Scaling`, `Orchestration`

---
**Curated for Prashant — Week 5 of INT332**


