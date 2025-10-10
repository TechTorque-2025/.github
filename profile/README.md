![Logo](Logo.png)

<h1 align="center">TechTorque 2025</h1>

<p align="center">
  <strong>The future of automobile service and appointment management.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Project%20Status-Active%20Development-success?style=for-the-badge" alt="Project Status"/>
  <img src="https://img.shields.io/badge/Version-v1.0%20(Scaffolded)-blue?style=for-the-badge" alt="Version"/>
  <img src="https://img.shields.io/badge/Assignment-Enterprise%20Application%20Development-lightgrey?style=for-the-badge" alt="Assignment"/>
</p>

---

### Technology Stack

<p align="center">
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white" alt="Spring Boot"/>
  <img src="https://img.shields.io/badge/go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white" alt="Go"/>
  <img src="https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white" alt="Next.js"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes"/>
</p>

---

Welcome to the central repository for the **TechTorque 2025** project. 

This project is a modern, enterprise-grade web application designed to digitize and streamline the operations of an automobile service company.

## 🏛️ System Architecture

![Architecture Diagram](Architecture.png)

The project is built on a **polyglot microservices architecture**. This design provides scalability, resilience, and technological flexibility, allowing each component to use the best tool for its specific job.

-   **💻 Frontend Web App:** A [Next.js](https://nextjs.org/) and TypeScript application serving both customers and employees.
-   **🌐 API Gateway:** A single entry point written in Go, responsible for routing, authentication (JWT validation), and rate limiting.
-   **⚙️ Backend Microservices:** A suite of independent [Spring Boot](https://spring.io/projects/spring-boot) services, each with its own dedicated PostgreSQL database, handling specific business domains
-   **🗄️ Databases:** A mix of [PostgreSQL](https://www.postgresql.org/) for transactional data and [MongoDB](https://www.mongodb.com/) for semi-structured data like notifications and chat logs.

For a complete architectural overview, please see the `EAD TechTorque.pdf` design document.

## 🚀 Getting Started: The All-in-One Development Environment

The entire TechTorque ecosystem is orchestrated using Docker Compose. This allows any developer to build and run all containers with a single command.

### ✅ Prerequisites

-   [Docker](https://www.docker.com/get-started) & [Docker Compose](https://docs.docker.com/compose/install/)
-   A Java 17+ JDK
-   Node.js & npm
-   Go Language

### ▶️ Running the Full System

1.  **Clone this repository.**
2.  **Navigate to the project root** (where this `README.md` and `docker-compose.yml` are located).
3.  **Run the Docker Compose command:**

    ```bash
    # To start all services and watch for code changes (recommended for development)
    docker-compose watch
    ```
    *or*
    ```bash
    # To start all services in the background without hot-reloading
    docker-compose up --build -d
    ```
This command will build, create, and start all containers.

###  Accessing the System

-   **API Gateway:** `http://localhost:8080`
-   **Frontend Application:** `http://localhost:3000` (after running `npm run dev` in the `Frontend_Web` directory)
-   **Individual Service Docs:** `http://localhost:[PORT]/swagger-ui.html` (e.g., `http://localhost:8081/swagger-ui.html` for the Auth Service).

## 🧩 Repository Structure

Each major component of the system resides in its own top-level directory. Please refer to the `README.md` file within each directory for specific details about that service.


### 🧑‍💻 Development Team

| Name | Role | GitHub |
|---|---|---|
| Randitha (B.H.A.R. Kulasekera) | Group Leader / Project Architect / Full Stack Developer / DevOps | [RandithaK](https://github.com/RandithaK) |
| Suweka | Full Stack Developer | [Suweka](https://github.com/Suweka) |
| Akith | Full Stack Developer | [Akith-002](https://github.com/Akith-002) |
| Pramudi | Full Stack Developer | [Pramudi02](https://github.com/Pramudi02) |
| Aditha | Full Stack Developer | [AdithaBuwaneka](https://github.com/AdithaBuwaneka) |
| Chamodi | Full Stack Developer | [ChamodiSandunika](https://github.com/ChamodiSandunika) |
| Dhanuja | Full Stack Developer / Project Manager | [Dhanuja416](https://github.com/Dhanuja416) |
| Mahesh | Full Stack Developer | [TharinduMahesh](https://github.com/TharinduMahesh) |
| Rothila | Full Stack Developer / Frontend Designer | [mehara-rothila](https://github.com/mehara-rothila) |
| Dinith | Full Stack Developer | [DinithEdirisinghe](https://github.com/DinithEdirisinghe) |


---
© 2025 TechTorque
