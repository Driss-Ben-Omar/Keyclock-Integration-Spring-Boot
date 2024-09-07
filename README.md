# Keycloak Integration with Spring Boot

## Description

This project demonstrates how to integrate Keycloak with a Spring Boot application to manage authentication and authorization using JWT (JSON Web Token). Keycloak is an open-source identity and access management solution that provides features such as authentication, authorization, and user management.

## Features

- User authentication with Keycloak.
- Role-based authorization using roles defined in Keycloak.
- Protection of REST APIs with JWT.
- Separation of access rights between different roles (`client_user` and `client_admin`).

## Prerequisites

Before starting, ensure you have the following installed on your machine:

- Java 17 or higher
- Maven 3.8.1 or higher
- Docker (to run Keycloak)
- Keycloak (can be run via Docker)

## Configuration

### Keycloak Setup

1. **Download and run Keycloak using Docker:**

   ```bash
   docker run -p 8080:8080 --name keycloak -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin quay.io/keycloak/keycloak:latest start-dev
