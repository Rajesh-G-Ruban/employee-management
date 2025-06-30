# 🧑‍💼 Employee Management System – Microservices Architecture

A scalable, cloud-ready **Employee Management System** built using **Java 11 + Spring Boot Microservices**, JWT authentication, Docker, and PostgreSQL/MySQL. This project follows enterprise patterns suitable for HRMS, admin portals, and SaaS apps.

---

## 🚀 Tech Stack

| Layer        | Technology                            |
|--------------|----------------------------------------|
| Backend      | **Java 11**, Spring Boot 2.7+, Spring Web |
| Architecture | Microservices (Eureka, Config Server)  |
| Security     | Spring Security, JWT                   |
| Database     | PostgreSQL / MySQL                     |
| Messaging    | RabbitMQ (optional)                    |
| Orchestration| Docker, Docker Compose                 |
| Monitoring   | Prometheus, Grafana                    |
| File Storage | Local | external if required           |
| Logging      | Spring Boot Logging / ELK Stack        |

---

## 📦 Microservices

| Service            | Description                                      |
|--------------------|--------------------------------------------------|
| `api-gateway`      | Central API gateway for routing & auth filtering |
| `config-server`    | Centralized config management                    |
| `eureka-server`    | Service registry                                 |
| `employee-service` | Manages employee records, CRUD                   |
| `project-service`  | Manages projects and assign projects             |
| `deparment-service`| deparment projects and mappig employee-department|
| `user-service`     | Auth, user, and role management                  |
| `file-service`     | File uploads like profile, etc..                 |
| `notification-service` | Email/SMS via RabbitMQ            |

---

## ✅ Features

- 🧾 Employee & Branch CRUD operations
- 🔐 JWT-based authentication and role-based access
- 🧑‍💼 Role management: `ADMIN`, `HR`, `USER`
- 🕵️ Soft deletes, audit logs, optimistic locking (`@Version`)
- 📄 File upload
- 🗃️ Supports both PostgreSQL and MySQL
- 🐳 Docker for local development and multi-service orchestration

---

## 🛠️ Setup Instructions

### 📋 Prerequisites

- Java 11
- Maven
- Docker & Docker Compose

### 🚀 Run the Project

1. Clone the repository:

```bash
git clone https://github.com/your-username/employee-management-microservices.git
cd employee-management-microservices
