<div align="center">

<img src="logoApp(1).png" width="110" alt="BrewBite Logo" />

# BrewBite Admin — Backend API

Backend API for the administrative panel of **BrewBite**, a café and bakery ordering platform.

[![Java](https://img.shields.io/badge/Java-17-ED8B00?style=flat&logo=openjdk&logoColor=white)](https://www.java.com)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-6DB33F?style=flat&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Primary%20DB-4169E1?style=flat&logo=postgresql&logoColor=white)](https://www.postgresql.org)
[![Cloudinary](https://img.shields.io/badge/Cloudinary-Media%20Storage-3448C5?style=flat&logo=cloudinary&logoColor=white)](https://cloudinary.com)
[![JWT](https://img.shields.io/badge/JWT-Auth-black?style=flat&logo=jsonwebtokens)](https://jwt.io)
[![Swagger](https://img.shields.io/badge/Swagger-API%20Docs-85EA2D?style=flat&logo=swagger&logoColor=black)](https://swagger.io)

</div>

---

## Overview

BrewBite Admin Backend is a secure RESTful API that powers the admin panel of the BrewBite platform. It supports core business operations such as item management, order processing, revenue tracking, customer feedback, complaints, and analytics.

---

## Features

- Admin registration and login
- JWT-based authentication
- Role-based access control
- Item creation, update, and deletion
- Item category and image management
- Order viewing and status updates
- Revenue calculation and reporting
- Ratings and reviews handling
- Comments and admin replies
- Complaint tracking and resolution
- Business analytics and statistics

---

## Tech Stack

- Java 17
- Spring Boot
- Spring Security
- Spring Data JPA
- Hibernate
- JWT Authentication
- PostgreSQL
- Cloudinary
- Swagger / OpenAPI
- Postman

---

## Architecture

<p align="center">
  <img src="Architecture.png" alt="BrewBite Admin Backend Architecture" width="100%" />
</p>

The project follows a layered architecture with clear separation between controllers, services, repositories, and database access.

---

## Project Structure

```text
src/main/java/com/brewbite/admin/
├── auth
├── item
├── order
├── revenue
├── rating
├── comment
├── complaint
├── analytics
└── common
