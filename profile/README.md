<p align="center">
  ![Logo](Logo.png)
</p>

<h1 align="center">TechTorque 2025</h1>

<p align="center">
  <strong>The future of automobile service and appointment management.</strong>
</p>

---

Welcome to the central repository for the **TechTorque 2025** project. This project is a modern, enterprise-grade web application designed to digitize and streamline the operations of an automobile service company.

## 🏛️ System Architecture

The project is built on a **polyglot microservices architecture**. This design provides scalability, resilience, and technological flexibility, allowing each component to use the best tool for its specific job.

-   **💻 Frontend Web App:** A Next.js and TypeScript application serving both customers and employees.
-   **🌐 API Gateway:** A single entry point written in Go, responsible for routing, authentication (JWT validation), and rate limiting.
-   **⚙️ Backend Microservices:** A suite of 7+ independent Spring Boot services, each with its own dedicated PostgreSQL database.
-   **🗄️ Databases:** A mix of PostgreSQL for transactional data and MongoDB for semi-structured data (notifications, chat logs).

For a complete architectural overview, please see the `EAD TechTorque.pdf` design document.

## 🚀 Getting Started: The All-in-One Development Environment

The entire TechTorque ecosystem is orchestrated using Docker Compose. This allows any developer to build and run all 11+ containers with a single command.

### Prerequisites

-   [Docker](https://www.docker.com/get-started) & [Docker Compose](https://docs.docker.com/compose/install/)
-   A Java 17+ JDK
-   Node.js & npm

### Running the Full System

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

### ઍ Accessing the System

-   **API Gateway:** `http://localhost:8080`
-   **Frontend Application:** `http://localhost:3000` (after running `npm run dev` in the `Frontend_Web` directory)
-   **Individual Service Docs:** `http://localhost:[PORT]/swagger-ui.html` (e.g., `http://localhost:8081/swagger-ui.html` for the Auth Service).

## 🧩 Repository Structure

Each major component resides in its own top-level directory. Please refer to the `README.md` file within each directory for specific details.