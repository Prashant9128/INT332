# 🏛️ Week 4: Architecture Evolution (Monolithic vs Microservices)

Welcome to **Week 4** of INT332! This module takes a step back to look at the big picture: how application architectures evolved to require containers in the first place. 

---

## 📑 Table of Contents
1. [Evolution of Application Architecture](#1-evolution-of-application-architecture)
2. [Monolithic Architecture](#2-monolithic-architecture)
3. [Microservices Architecture](#3-microservices-architecture)
4. [Monolithic vs Microservices](#4-monolithic-vs-microservices)
5. [🎓 Interview Prep & Revision](#5-interview-prep--revision)

---

## 1. 🕰️ Evolution of Application Architecture

### 1980s - Mid 1990s
* **Physical servers** inside data centers
* **Monolithic** applications
* **Waterfall** development model
* **Characteristics:** Large single applications, difficult maintenance, slow deployment.

### Late 1990s - 2000s
* **Virtualization** introduced (VMWare, KVM)
* **N-tier** applications
* **Agile** methodologies
* **Improvements:** Better resource utilization, faster development cycle, easier deployment than physical servers.

### 2010 - Present
* **Cloud computing**
* **Microservices** architecture
* **Containers** (Docker)
* **Kubernetes** orchestration
* **DevOps** culture
* **Features:** Faster deployment, better scalability, independent services, high availability.

---

## 2. 🏢 Monolithic Architecture

### Definition
A monolithic application is a single large application where all components are tightly connected and deployed together.

### Structure of Monolithic Application

![Monolithic Architecture](./images/monolithic.png)
*All modules exist inside one application.*

### ✨ Components of Monolithic Application
1. **User Interface (UI)**
   * **Example:** Shopping website pages, Mobile app screens
   * **Technologies:** HTML, CSS, JavaScript
   * **Purpose:** Interacts with users, displays information, takes user input
2. **Data Access Layer**
   * **Example:** ProductDAO class, SQL query handling modules
   * **Technologies:** JDBC, SQLAlchemy, Entity Framework
   * **Purpose:** Communicates with database, reads/writes data
3. **Data Store**
   * **Example:** MySQL, PostgreSQL
   * **Purpose:** Stores application data, retrieves data when needed

> [!TIP]
> **Advantages:**
> * **Simple Deployment:** Only one application deployed
> * **Easier Testing:** End-to-end testing simpler
> * **Better Performance:** Components communicate directly in memory
> * **Easy Initial Development:** Good for small applications

> [!WARNING]
> **Disadvantages:**
> * **Scalability Problem:** Entire application must scale together
> * **Difficult Maintenance:** Large codebase becomes hard to manage
> * **Technology Barrier:** Hard to introduce new technology
> * **Difficult Understanding:** New developers struggle to understand large systems

---

## 3. 🧩 Microservices Architecture

### Definition
Microservices divide an application into small independent services that communicate with each other using APIs.

### Structure of Microservices Application

![Microservices Architecture](./images/microservices.png)

### 🚀 Key Concepts of Microservices

1. **Smaller Independent Services**
   * *Example (Online Shopping App):* User Service, Order Service, Payment Service, Inventory Service. Each service performs one specific task.
2. **Business Goal Based Design**
   * Each microservice focuses on one business function.
   * *Example:* Payment Service → Handles payments, Inventory Service → Manages stock, User Service → Authentication.
3. **Communication Between Services**
   * Services communicate using REST APIs or Message Queues.
   * *Example:* `POST /payment/process`
4. **Separate Database Per Service**
   * *Benefit:* Loose coupling, independent scaling, better flexibility.

> [!NOTE]
> **Advantages of Microservices:**
> * **Scalability:** Scale only required services
> * **Independent Deployment:** Deploy one service without affecting others
> * **Technology Flexibility:** Different languages/tools possible
> * **Fault Isolation:** Failure of one service doesn't crash whole system
> * **Faster Development:** Multiple teams work independently
> * **Easier Maintenance:** Small codebases easier to debug

---

## 4. ⚖️ Monolithic vs Microservices

| Feature | Monolithic | Microservices |
| :--- | :--- | :--- |
| **Structure** | Single application | Multiple services |
| **Deployment** | One deployment | Independent deployment |
| **Scalability** | Entire app scaled | Individual service scaling |
| **Failure Impact** | Entire app affected | Only one service affected |
| **Maintenance** | Difficult in large systems | Easier |
| **Technology Choice** | Limited | Flexible |

---

## 5. 🎓 Interview Prep & Revision

### Real-World Examples
| Platform | Architecture |
| :--- | :--- |
| Old desktop ERP | Monolithic |
| Netflix | Microservices |
| Amazon | Microservices |
| Flipkart | Microservices |

### 🚀 One-Line Revision Notes
* **Monolith** = One big application
* **Microservices** = Many small services
* **REST API** = How microservices talk to each other
* **Loose Coupling** = Services are independent

### 📝 Important Interview / Viva Questions
**Q1. Difference between Monolithic and Microservices?**
* **Monolithic** = Single large application
* **Microservices** = Small independent services

> [!IMPORTANT]
> **Important Keywords to Remember:**
> `Monolithic Architecture`, `Microservices`, `REST API`, `Loose Coupling`, `Service Discovery`, `DevOps`

---
**Prepared for CA-1 Exam by Prashant**
