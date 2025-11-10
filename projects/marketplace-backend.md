# Marketplace Backend — Freelance Services Platform

## Project Summary
Marketplace Backend supports the lifecycle of freelance service listings, product sales, and user interactions. The system enables role-based access, transaction tracking, and review workflows to connect buyers with specialized professionals.

## Core Capabilities
- 📋 **Listings & Catalog:** Create, update, and manage services or products across multiple categories.
- 🛒 **Purchases & Orders:** Handle order placement, payment coordination, and delivery tracking.
- ⭐ **Ratings & Reviews:** Collect qualitative and quantitative feedback to boost marketplace trust.
- 🛡️ **Roles & Permissions:** Enforce authentication and authorization policies tailored to administrators, sellers, and buyers.

## Tech Stack
- **Java 21** with **Spring Boot 3.4.1** as the backbone framework
- **Spring Data JPA** with **MySQL** for relational data and **MongoDB** for complementary document storage
- **Spring Security** configuration with DTO-based service layers and controller validation
- **Maven**-managed build with extensive integration testing via Postman collections

## Project Structure
```
src/main/java/ec/edu/uce/marketplace
├── config         # Security configuration and shared properties
├── controllers    # REST endpoints
├── dtos           # Data transfer objects
├── entities       # Domain entities
├── exceptions     # Custom exception handling
├── repositories   # Persistence interfaces
├── security       # Authentication/authorization components
├── services       # Business logic services
├── utils          # Auxiliary helpers
```

## Development Notes
- GitHub for version control and collaborative workflows.
- Postman suites used to exercise endpoints during development.
- Documentation and onboarding materials maintained in the repository README.
