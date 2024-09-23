# Software Development Lifecycle for Machine Learning Enabled Systems

## Introduction
This repository is part of a thesis project focused on exploring and implementing the Software Development Lifecycle (SDLC) specifically tailored for Machine Learning (ML) enabled systems. The project aims to address the unique challenges and requirements of ML systems, from initial design through development, deployment, and maintenance.

## Project Architecture
The project uses a microservices architecture to ensure scalability, flexibility, and robust separation of concerns. Below is a breakdown of each service within our system:

### Services
- **Database Service:** Manages all database operations using MongoDB, initialized with specific configurations and scripts.
- **Backend Service:** Acts as the nerve centre for processing and business logic, interfacing with the database and other services.
- **Medical Analysis Service:** Dedicated to processing medical data, providing analytics and insights.
- **Medical Risk Calculation Service:** Computes risk assessments based on medical data.
- **Frontend Service:** Serves the user interface, facilitating user interaction with our system.
- **Reverse Proxy Service (SWAG):** Manages external access to our services with SSL termination and request routing.

## Docker Configuration
```yaml
# YAML configuration snippet provided here for quick reference
version: "3.3"
services:
  # MongoDB service
  ...
  # Backend service
  ...
  # Additional service configurations follow the same pattern
```

### Highlighted Features:
- **Security and Configuration:** Each service is configured with environment variables for secure operation, including database credentials, JWT secrets, and encryption keys.
- **Resilience and Scalability:** Services such as the medical analysis and risk calculation are designed to restart unless stopped, ensuring high availability.

## Installation and Setup
Instructions for setting up the project locally using Docker:
1. Ensure Docker and Docker-compose are installed on your system.
2. Clone this repository.
3. Run `docker-compose up` from the repository's root to start all services.

## Contributing
Upon request.

## License
None
