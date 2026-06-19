# DeepSkyn — Skincare Routine App Backend

> A RESTful backend API powering DeepSkyn, a personalized skincare routine application that helps users build and manage their daily skincare regimens.

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

---

## Overview

DeepSkyn is a skincare routine management platform that allows users to discover, build, and track personalized skincare routines. This repository contains the backend API responsible for user management, product data, routine scheduling, and skin profile analysis.

Built as a team project by **Dev-Masters**.

## Features

- User registration, authentication, and profile management
- Skin type profiling and personalized routine recommendations
- Product catalog with ingredients and usage instructions
- Routine builder — morning and evening schedules
- Progress tracking and routine history
- RESTful API designed for mobile and web clients

## Project Structure

```
DeepSkynBackEnd_ByDev-Masters/
├── src/
│   └── main/
│       ├── java/          # Application source code
│       └── resources/     # Configuration files
├── Dockerfile             # Container image definition
├── pom.xml                # Maven build configuration
└── README.md
```

## Tech Stack

| Component | Technology |
|-----------|-----------|
| Language | Java |
| Framework | Spring Boot |
| Build Tool | Maven |
| Containerization | Docker |
| Authentication | JWT |
| Database | MySQL / PostgreSQL |

## Getting Started

### Prerequisites

- Java 17+
- Maven 3.8+
- Docker (optional)

### Run Locally

```bash
# Clone the repository
git clone https://github.com/HamzaDalhoumi/DeepSkynBackEnd_ByDev-Masters.git
cd DeepSkynBackEnd_ByDev-Masters

# Build and run
./mvnw spring-boot:run
```

The API will be available at `http://localhost:8080`.

### Run with Docker

```bash
docker build -t deepskyn-backend .
docker run -p 8080:8080 deepskyn-backend
```

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Authenticate and get token |
| GET | `/api/users/{id}/profile` | Get user skin profile |
| GET | `/api/routines` | Get user's routines |
| POST | `/api/routines` | Create a new routine |
| GET | `/api/products` | Browse product catalog |
| GET | `/api/products/{id}` | Get product details |

## Team

Built by **Dev-Masters**

- [Hamza Dalhoumi](https://github.com/HamzaDalhoumi)

---

*DeepSkyn — Know your skin. Build your routine.*
