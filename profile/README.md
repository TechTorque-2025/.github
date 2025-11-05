# TechTorque 2025

![Logo](Logo.png)

**The future of automobile service and appointment management.**

![Project Status](https://img.shields.io/badge/Project%20Status-Active%20Development-yellow?style=for-the-badge) ![Version](https://img.shields.io/badge/Version-v1.0%20(14%25%20Complete)-orange?style=for-the-badge) ![Assignment](https://img.shields.io/badge/Assignment-Enterprise%20Application%20Development-lightgrey?style=for-the-badge)

**📊 Latest Audit:** November 5, 2025 | **🎯 Completion:** 14/98 Endpoints (14%) | **⚠️ Status:** Critical Issues Identified

---

## 🚨 Project Status Update (November 2025)

> **Comprehensive audit completed.** See [`PROJECT_AUDIT_REPORT_2025.md`](../../PROJECT_AUDIT_REPORT_2025.md) for full details.

### Quick Status Summary

| Aspect | Status | Grade |
|--------|--------|-------|
| **Architecture** | ✅ Excellent | A |
| **Implementation** | ⚠️ 14% Complete | D |
| **Security** | ✅ Good Foundation | B |
| **Data Consistency** | ❌ Critical Issues | F |
| **Production Ready** | ❌ No | N/A |

### Critical Issues Identified

1. ❌ **Notification Service Missing** (Production Blocker)
2. ❌ **70% of Endpoints are Stubs** (No Business Logic)
3. ❌ **Data Seeders Missing** (5 of 7 services)
4. ⚠️ **Authentication Incomplete** (Missing email verification, password reset)

### What Works

- ✅ Authentication service has solid RBAC foundation (56% complete)
- ✅ API Gateway configured and routing correctly
- ✅ All controller skeletons properly structured
- ✅ Security annotations and JWT validation working

### What Needs Work

- 🔥 **Priority 1:** Create Notification Service (0% complete)
- 🔥 **Priority 1:** Implement business logic for 55 stub endpoints
- 🔥 **Priority 1:** Fix data seeder consistency across services
- ⚠️ **Priority 2:** Complete authentication features
- ⚠️ **Priority 2:** Implement inter-service communication

**Estimated Time to Production:** 3 months (480 hours with 2 developers)

---

## Build status for the main repositories

[![Build and Test Vehicle Service](https://github.com/TechTorque-2025/Vehicle_Service/actions/workflows/buildtest.yaml/badge.svg)](https://github.com/TechTorque-2025/Vehicle_Service/actions/workflows/buildtest.yaml)

[![Build and Test Time Logging Service](https://github.com/TechTorque-2025/Time_Logging_Service/actions/workflows/buildtest.yaml/badge.svg)](https://github.com/TechTorque-2025/Time_Logging_Service/actions/workflows/buildtest.yaml)

[![Build and Test Project Service](https://github.com/TechTorque-2025/Project_Service/actions/workflows/buildtest.yaml/badge.svg)](https://github.com/TechTorque-2025/Project_Service/actions/workflows/buildtest.yaml)

[![Build and Test Payment Service](https://github.com/TechTorque-2025/Payment_Service/actions/workflows/buildtest.yaml/badge.svg)](https://github.com/TechTorque-2025/Payment_Service/actions/workflows/buildtest.yaml)

[![Build and Test Authentication Service](https://github.com/TechTorque-2025/Authentication/actions/workflows/buildtest.yaml/badge.svg)](https://github.com/TechTorque-2025/Authentication/actions/workflows/buildtest.yaml)

[![Build and Test Appointment Service](https://github.com/TechTorque-2025/Appointment_Service/actions/workflows/buildtest.yaml/badge.svg)](https://github.com/TechTorque-2025/Appointment_Service/actions/workflows/buildtest.yaml)

[![Build and Test Admin Service](https://github.com/TechTorque-2025/Admin_Service/actions/workflows/buildtest.yaml/badge.svg)](https://github.com/TechTorque-2025/Admin_Service/actions/workflows/buildtest.yaml)

[![Build and Test API Gateway](https://github.com/TechTorque-2025/API_Gateway/actions/workflows/buildtest.yaml/badge.svg)](https://github.com/TechTorque-2025/API_Gateway/actions/workflows/buildtest.yaml)

[![Build and Test Frontend_Web](https://github.com/TechTorque-2025/Frontend_Web/actions/workflows/buildtest.yaml/badge.svg)](https://github.com/TechTorque-2025/Frontend_Web/actions/workflows/buildtest.yaml)

---

## Technology Stack

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white) ![Go](https://img.shields.io/badge/go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white) ![Next.js](https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)

---

Welcome to the central repository for the **TechTorque 2025** project.

This project is a modern, enterprise-grade web application designed to digitize and streamline the operations of an automobile service company.

## 🏛️ System Architecture

![Architecture Diagram](Architecture.png)

The project is built on a **polyglot microservices architecture**. This design provides scalability, resilience, and technological flexibility, allowing each component to use the best tool for its specific job.

- **💻 Frontend Web App:** A [Next.js](https://nextjs.org/) and TypeScript application serving both customers and employees.
- **🌐 API Gateway:** A single entry point written in Go, responsible for routing, authentication (JWT validation), and rate limiting.
- **⚙️ Backend Microservices:** A suite of independent [Spring Boot](https://spring.io/projects/spring-boot) services, each with its own dedicated PostgreSQL database, handling specific business domains.
- **🗄️ Databases:** A mix of [PostgreSQL](https://www.postgresql.org/) for transactional data and [MongoDB](https://www.mongodb.com/) for semi-structured data like notifications and chat logs.

For a complete architectural overview, please see the `EAD TechTorque.pdf` design document.

## 🚀 Getting Started: The All-in-One Development Environment

The entire TechTorque ecosystem is orchestrated using Docker Compose. This allows any developer to build and run all containers with a single command.

### ✅ Prerequisites

- [Docker](https://www.docker.com/get-started) & [Docker Compose](https://docs.docker.com/compose/install/)
- A Java 17+ JDK
- Node.js & npm
- Go language

### ▶️ Running the Full System

1. **Clone this repository.**
2. **Navigate to the project root** (where this `README.md` and `docker-compose.yml` are located).
3. **Run the Docker Compose command:**

```bash
# To start all services and watch for code changes (recommended for development)
docker-compose watch
```

or

```bash
# To start all services in the background without hot-reloading
docker-compose up --build -d
```

This command will build, create, and start all containers.

### Accessing the System

- **API Gateway:** `http://localhost:8080`
- **Frontend Application:** `http://localhost:3000` (after running `npm run dev` in the `Frontend_Web` directory)
- **Individual Service Docs:** `http://localhost:[PORT]/swagger-ui.html` (e.g., `http://localhost:8081/swagger-ui.html` for the Auth Service)

## 🧩 Repository Structure

Each major component of the system resides in its own top-level directory. Please refer to the `README.md` file within each directory for specific details about that service.

### Service Completion Status

| Service | Port | Endpoints | Status | Grade | Blocker Issues |
|---------|------|-----------|--------|-------|----------------|
| 🔐 **Authentication** | 8081 | 14/25 (56%) | 🟡 Partial | B- | Missing: Email verification, Token refresh, Password reset |
| 🚗 **Vehicle Management** | 8082 | 0/7 (0%) | 🔴 Stub | D | Missing: All business logic, Data seeder |
| 📅 **Appointment** | 8083 | 0/9 (0%) | 🔴 Stub | D | Missing: All business logic, Data seeder, Calendar view |
| 🔧 **Service/Project** | 8084 | 0/16 (0%) | 🔴 Stub | D- | Missing: Create service endpoint, Invoice link |
| ⏱️ **Time Logging** | 8085 | 0/7 (0%) | 🔴 Stub | D | Missing: All business logic, Data consistency |
| 💳 **Payment** | 8086 | 0/6 (0%) | 🟡 Partial | D+ | Missing: Business logic (PayHere 60% done) |
| 👤 **Admin** | 8087 | 0/18 (0%) | 🔴 Stub | D- | Missing: All business logic, Data seeder |
| 🔔 **Notification** | N/A | 0/5 (0%) | ❌ Missing | F | **PRODUCTION BLOCKER - Service doesn't exist** |
| 🤖 **AI Chatbot** | N/A | 0/4 (0%) | ⚪ Not Started | N/A | Bonus feature - Not required for MVP |
| 🌐 **WebSocket** | N/A | 0/1 (0%) | ⚪ Not Started | N/A | Enhancement - Not critical |

**Overall Implementation:** 14/98 endpoints fully implemented (14%)

### Data Seeder Status

| Service | Seeder | Quality | Issues |
|---------|--------|---------|--------|
| Authentication | ✅ Yes | A+ | Excellent - Profile-based, comprehensive |
| Time Logging | ✅ Yes | B | Good but uses hardcoded IDs (EMP001, EMP002) |
| Vehicle | ❌ No | F | **CRITICAL:** Cannot test appointments |
| Appointment | ❌ No | F | **CRITICAL:** No service types defined |
| Service/Project | ❌ No | F | **CRITICAL:** Cannot test workflows |
| Payment | ❌ No | F | Cannot test payment flows |
| Admin | ❌ No | F | No service type configuration |

**Data Consistency Grade: F** (Only 2 of 7 services have seeders)

## 🧑‍💻 Development Team

| Name | Role | GitHub |
|---|---:|---|
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

## 🚀 Critical Path Forward

### Phase 1: Foundation (Weeks 1-2) 🔥 CRITICAL

**Objective:** Fix data consistency and core infrastructure

- [ ] **Create Data Seeders for All Services**
  - Vehicle Service: 2-3 vehicles per customer
  - Appointment Service: Service types (Oil Change, Brake Service, etc.)
  - Project Service: Sample projects and quotes
  - Payment Service: Sample invoices and payments
  - Admin Service: Service type configuration

- [ ] **Establish Shared Constants Module**
  - Create `common-constants` library
  - Define fixed UUIDs for seed data
  - Document UUID mapping across services

- [ ] **Complete Critical Auth Features**
  - Email verification flow
  - JWT refresh token endpoint
  - Password reset flow (forgot/reset)
  - Profile update endpoints

### Phase 2: Core Business Logic (Weeks 3-5) 🔥 CRITICAL

**Objective:** Implement essential workflows

- [ ] **Service Management**
  - POST `/services` - Create service from appointment
  - Implement service status management
  - Add invoice generation
  - Link Service → Payment services

- [ ] **Vehicle Service Complete**
  - Implement all CRUD operations
  - Photo upload/storage functionality
  - Service history tracking

- [ ] **Appointment Service Complete**
  - Booking logic with slot validation
  - Availability calculation algorithm
  - Employee schedule views
  - Monthly calendar endpoint

### Phase 3: Notification Service (Weeks 6-7) 🚨 BLOCKER

**Objective:** Create missing notification service

- [ ] **Build Notification Service** (Port 8088)
  - Set up Spring Boot service
  - Implement notification CRUD
  - Email notification system
  - Push notification subscriptions
  - Integrate with all services

**⚠️ Production cannot launch without this service**

### Phase 4: Complete Implementation (Weeks 8-10) ⚠️ HIGH

**Objective:** Finish all remaining services

- [ ] **Time Logging Service** - Implement all endpoints
- [ ] **Payment Service** - Complete PayHere integration
- [ ] **Project Management** - Complete quote workflows
- [ ] **Admin Service** - Implement WebClient proxies and reporting

### Phase 5: Testing & Security (Weeks 11-12) ⚠️ HIGH

**Objective:** Production readiness

- [ ] Integration tests for critical workflows
- [ ] Security audit and hardening
- [ ] Performance testing
- [ ] Documentation completion

**Estimated Completion:** February 2026 (3 months)

---

## 📋 Key Audit Findings

### Strengths ✅

1. **Excellent Architecture** - Clean microservices with clear boundaries
2. **Security Foundation** - JWT auth, RBAC, password encryption working
3. **Code Organization** - Consistent package structure across services
4. **API Gateway** - Properly configured and routing correctly
5. **Auth Service** - Most complete service (56% done)

### Critical Issues ❌

1. **Missing Notification Service** - Production blocker, 0% complete
2. **Stub Endpoints** - 70% of endpoints have no business logic
3. **Data Consistency** - Only 2/7 services have seeders
4. **Inter-Service Communication** - Not established
5. **Authentication Incomplete** - Missing email verification, password reset

### Security Concerns ⚠️

1. **JWT Secret Hardcoded** - High risk in production
2. **No Token Refresh** - Will cause session issues
3. **No Email Verification** - Anyone can register
4. **No Rate Limiting** - Vulnerable to DoS attacks

### Recommendations 💡

**Immediate Actions (This Week):**
1. Create data seeders for all services
2. Implement POST `/services` endpoint
3. Start Notification Service development
4. Externalize JWT secret to environment variable

**Next Month:**
1. Complete core workflows (Vehicle → Appointment → Service → Payment)
2. Finish authentication features
3. Complete Notification Service
4. Add integration tests

**Before Production:**
1. Security audit and penetration testing
2. Performance and load testing
3. Backup/restore testing
4. Complete API documentation
5. Set up monitoring and alerts

---

## 📊 Detailed Metrics

### Endpoint Implementation by Category

| Category | Total | Implemented | Stubs | Missing | % Complete |
|----------|-------|-------------|-------|---------|------------|
| Authentication & Users | 25 | 14 | 0 | 11 | 56% |
| Vehicle Management | 7 | 0 | 7 | 0 | 0% |
| Appointments | 9 | 0 | 8 | 1 | 0% |
| Services & Projects | 16 | 0 | 14 | 2 | 0% |
| Time Logging | 7 | 0 | 7 | 0 | 0% |
| Payments & Billing | 6 | 0 | 6 | 0 | 0% |
| Admin & Reports | 18 | 0 | 13 | 5 | 0% |
| Notifications | 5 | 0 | 0 | 5 | 0% |
| **TOTAL** | **98** | **14** | **55** | **29** | **14%** |

### Implementation Status Visualization

```
Overall Progress: ■■□□□□□□□□□□□□□□□□□□ 14%
                  └─ 14 Fully Implemented
                  └─ 55 Stubs (No Logic)
                  └─ 29 Missing

Service Health:
Authentication   ■■■■■■■■■■■□□□□□□□□□ 56% (B-)
Vehicle          ■□□□□□□□□□□□□□□□□□□□ 0%  (D)
Appointment      ■□□□□□□□□□□□□□□□□□□□ 0%  (D)
Service/Project  ■□□□□□□□□□□□□□□□□□□□ 0%  (D-)
Time Logging     ■□□□□□□□□□□□□□□□□□□□ 0%  (D)
Payment          ■■□□□□□□□□□□□□□□□□□□ 10% (D+)
Admin            ■□□□□□□□□□□□□□□□□□□□ 0%  (D-)
Notification     □□□□□□□□□□□□□□□□□□□□ 0%  (F) MISSING
```

---

## 📚 Documentation

- [Complete API Design](../../complete-api-design.md) - Full API specification
- [System Design Document](../../System%20Design.txt) - Architecture overview
- [Audit Report](../../PROJECT_AUDIT_REPORT_2025.md) - **Comprehensive project audit**
- [Endpoint Implementation Report](../../ENDPOINT_IMPLEMENTATION_REPORT.md) - Previous status

---
© 2025 TechTorque
