# Safe Map Backend — Microservices Architecture

## Overview
Safe Map empowers citizens and city officials to register, visualize, and monitor protected areas across urban zones with elevated crime rates. The platform aggregates crowd-sourced safety data, schedules optimal visiting windows, and highlights historical events tied to each location.

## Tech Stack
- **Java 17** with **Spring Boot 3.2+** across modular services
- **Spring Cloud** suite (Eureka, Config Server, Gateway) for service discovery and centralized configuration
- **MongoDB** for document-oriented persistence and geolocated safe place records
- **Spring Security** with JWT authentication, plus Swagger/OpenAPI documentation
- **Docker & Docker Compose** to orchestrate the microservice environment

## Microservices Landscape
```
safe-map-backend/
├── config-server/      # Centralized configuration
├── eureka-server/      # Service discovery (registry)
├── gateway/            # API Gateway
├── user-service/       # Users and authentication
├── safeplace-service/  # Places marked as safe
├── schedule-service/   # Safe time ranges per place
├── event-service/      # Events logged per location
├── docker/             # Docker Compose + environment
└── pom.xml             # Parent POM
```

## Highlights
- Microservice isolation enables independent scaling of user, place, schedule, and event domains.
- Centralized gateway exposes a unified API layer secured with JWT tokens.
- Dockerized toolchain streamlines local development and multi-service deployments.
