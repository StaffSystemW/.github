![.NET](https://img.shields.io/badge/.NET-8-blue)
![React](https://img.shields.io/badge/React-TypeScript-blue)
![CI](https://img.shields.io/badge/CI-GitHub_Actions-green)
![Docker](https://img.shields.io/badge/Docker-ready-blue)
![License](https://img.shields.io/badge/license-MIT-lightgrey)
![Tests](https://img.shields.io/badge/tests-passing-brightgreen)

# WorkShift

A production-style **fullstack shift booking system** built with **.NET, React and modern DevSecOps practices**.

This project was built as my **final portfolio project during my .NET Fullstack YH education**.
Instead of building multiple small demos, I focused on creating **one realistic system that demonstrates how modern software is built, tested, secured and deployed.**

The project emphasizes:

* Clean architecture
* DevSecOps pipelines
* Automated testing
* Observability
* Scalable system design

The application is **publicly deployed** and can also be **run locally using Docker**.

---

## Quick Overview (for recruiters)

### Problem solved

Managing employee work shifts where:

* Admins create and manage shifts
* Employees can book available shifts
* The system handles authentication and authorization

### Tech Stack

**Backend**

* ASP.NET Web API
* Clean Architecture / Vertical Slice
* FluentValidation
* AutoMapper

**Frontend**

* React
* TypeScript
* React Query

**Infrastructure**

* YARP API Gateway
* Docker
* GitHub Actions CI/CD

**Observability**

* Serilog logging
* OpenTelemetry distributed tracing
* Health checks

**Testing**

* Unit tests
* Integration tests
* Testcontainers

---

## Live Demo

Frontend
`https://your-demo-url`

API Gateway
`https://your-api-url`

Swagger
`https://your-api-url/swagger`

---

## About Me

I am a soon-to-graduate **.NET Fullstack developer from a Swedish YH program**, currently looking for my **first junior developer role**.

My main interests are:

* Backend architecture
* DevSecOps
* Cloud-native systems
* Scalable application design

This project represents the **engineering practices I want to bring into my first development role**.

---

## System Architecture

High level architecture:

```
        ┌───────────────┐
        │   React App   │
        └───────┬───────┘
                │
                ▼
        ┌───────────────┐
        │   YARP Gateway│
        └───────┬───────┘
                │
                ▼
     ┌─────────────────────────┐
     │     ASP.NET Web APIs    │
     │  Clean / Vertical Slice │
     └─────────────┬───────────┘
                   │
                   ▼
               Database
```

### Design goals

* Maintainable architecture
* Strong separation of concerns
* Testability
* Cloud-ready infrastructure
* Observable systems

### Architectural principles

* SOLID
* Clean Architecture
* Vertical Slice Architecture
* API-first design

---

## Get Started

### Clone the repository

```bash
git clone https://github.com/yourusername/workshift.git
cd workshift
```

### Run locally with Docker

```bash
docker compose up --build
```

Services will start automatically.

```
Frontend: http://localhost:3000
API Gateway: http://localhost:8080
Swagger: http://localhost:8080/swagger
```

---

## Frontend

The frontend is built using **React and TypeScript** with a focus on maintainability and good UX patterns.

### Key Features

* Type-safe frontend using TypeScript
* Component-driven architecture
* React Query for server state management
* Dedicated API service layer
* Protected routes
* Form validation
* Error handling
* Loading states
* Responsive design
* Dark mode

### Example structure

```
frontend
│
├── components
├── pages
├── hooks
├── services
├── types
└── utils
```

---

## Backend

The backend consists of **ASP.NET Web APIs** designed around **Clean Architecture and Vertical Slice patterns**.

### Features

* RESTful CRUD endpoints
* FluentValidation request validation
* Global exception handling middleware
* AutoMapper object mapping
* Dependency injection
* Health checks
* Structured logging

### Development principles

* SOLID
* Separation of concerns
* Testability
* Maintainability

---

## API Gateway

The system uses **YARP (Yet Another Reverse Proxy)** as an API Gateway.

### Responsibilities

* Central entry point for APIs
* Request routing
* Service abstraction
* Future microservice expansion

This architecture allows easy evolution into a **microservice-based system**.

---

## Database

The application supports both **local and cloud databases**.

### Technologies

* Entity Framework Core
* Code-first migrations

### Core entities

* Users
* Shifts
* Bookings

---

## Testing Strategy

The project includes multiple layers of testing.

### Unit Tests

Focused on domain and business logic.

### Integration Tests

Tests API endpoints using real infrastructure.

### Testcontainers

Integration tests spin up real containers for dependencies to create reliable test environments.

### Tools

* xUnit
* Moq
* Testcontainers

---

## CI/CD Pipeline

The project uses **GitHub Actions** to implement a DevSecOps pipeline.

### Pipeline stages

```
Push / Pull Request
        │
        ▼
Lint
        │
        ▼
Unit Tests
        │
        ▼
Build
        │
        ▼
SBOM Generation
        │
        ▼
SAST / Code Quality
        │
        ▼
Dependency Scan
        │
        ▼
Docker Build
        │
        ▼
Deploy
```

This ensures the system is automatically:

* Tested
* Analyzed for vulnerabilities
* Built into containers
* Deployed

---

## Observability

Modern production systems require strong observability.

### Logging

* Serilog
* Structured logging

### Distributed Tracing

* OpenTelemetry
* Correlation IDs

This makes it possible to trace requests across services.

### Health Checks

Health endpoints are implemented for:

* Application services
* Containers
* Infrastructure

---

## Security Practices

Security considerations include:

* Authentication
* Protected routes
* Dependency vulnerability scanning
* SAST scanning in CI pipeline

---

## Use of AI

AI tools were used as **engineering assistance during development**, similar to modern development workflows.

Examples include:

* Debugging assistance
* Architecture brainstorming
* Documentation support

All generated suggestions were **reviewed and implemented manually**.

---

## Why This Project Exists

This project was created to demonstrate the ability to build software with:

* Real-world architecture
* DevSecOps workflows
* Automated testing
* Modern frontend practices
* Observability

It reflects the **kind of engineering environment I want to work in as a developer**.

---


```

```
