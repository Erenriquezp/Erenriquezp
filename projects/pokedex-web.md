# Pokédex Web — Reactive Pokémon Explorer

## Project Overview
Pokédex Web is a modern application for researching Pokémon data, displaying stats, sprites, and evolution chains with responsive, theme-aware pages. The platform blends real-time search with batch-preloaded datasets to keep navigation instant.

## Key Features
- 🔍 **Search & Detail Views:** Query Pokémon by name and surface complete profiles, including abilities, weight, height, and base experience.
- 📊 **Interactive Stats:** Render dynamic charts for HP, attack, defense, speed, and more with optimized pagination between entries.
- 🖼️ **Rich Media:** Present classic, Dream World, Home, official artwork, shiny, and alternate sprites with efficient caching.
- 🔄 **Evolution Chains:** Visualize multi-branch evolutions and conditional paths with intuitive UI cues.
- ⚡ **Performance:** Reactive WebFlux architecture, parallelized data ingestion, and MySQL-backed storage for sub-second responses.

## Tech Stack
- **Spring Boot**, **Spring WebFlux**, **Spring Data JPA**, **Hibernate**, **Spring Batch**, and **WebClient**
- **MySQL** for persistent storage with batch preloading flows
- **HTML5**, **CSS3**, **JavaScript**, and Fetch API-driven front-end
- Responsive UI using Bootstrap, dark/light theming, and smooth animations

## Project Structure
```
/pokedex-web
│── src/
│   ├── main/
│   │   ├── java/ec/edu/uce/pokedexweb/
│   │   │   ├── controller/    # REST Controllers
│   │   │   ├── models/        # JPA Entities
│   │   │   ├── repository/    # Database Repositories
│   │   │   ├── service/       # Business Logic Services
│   │   │   ├── config/        # Application Configuration
│   ├── resources/
│   │   ├── static/
│   │   │   ├── css/           # Stylesheets
│   │   │   ├── js/            # Frontend Logic
│   │   │   ├── pages/         # HTML Views
│   │   ├── templates/         # Thymeleaf Templates
│── pom.xml                    # Maven Dependencies
│── README.md                  # Documentation
```

## Getting Started
1. **Clone the repository** and move into the project directory.
2. **Provision the MySQL database** (`CREATE DATABASE pokedex_web;`) and update `application.properties` with credentials.
3. **Run** `mvn spring-boot:run` to start the reactive backend.
4. **Explore** the UI at `http://localhost:8080/pages/index.html` and REST endpoints such as `/api/pokemon/name/{name}`.
