<h1 style="text-align: left; display: flex;">
  <img src="https://raw.githubusercontent.com/Melikash98/BrewBiteApp/main/logoApp.png" alt="Logo" width="80px" height="80px" style="margin-right: 10px;" />
  BrewBite Admin — Backend API
</h1>

**RESTful backend for the administrative panel of the BrewBite café & bakery ordering platform**
[![Java](https://img.shields.io/badge/Java-17-ED8B00?style=flat&logo=openjdk&logoColor=white)](https://www.java.com)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-6DB33F?style=flat&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Primary%20DB-4169E1?style=flat&logo=postgresql&logoColor=white)](https://www.postgresql.org)
[![Redis](https://img.shields.io/badge/Redis-Cache-DC382D?style=flat&logo=redis&logoColor=white)](https://redis.io)
[![Cloudinary](https://img.shields.io/badge/Cloudinary-Media%20Storage-3448C5?style=flat&logo=cloudinary&logoColor=white)](https://cloudinary.com)
[![JWT](https://img.shields.io/badge/JWT-Auth-black?style=flat&logo=jsonwebtokens)](https://jwt.io)
[![Swagger](https://img.shields.io/badge/Swagger-API%20Docs-85EA2D?style=flat&logo=swagger&logoColor=black)](https://swagger.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---
##  Overview

**BrewBite Admin Backend** is the server-side engine powering the admin panel of the [BrewBite Android App](https://github.com/Melikash98/BrewBiteApp) — a full-featured ordering application for cafés and bakeries.

While the Android app handles the customer-facing experience (browsing menu, placing orders, and payment), this backend gives the **admin complete control** over the entire business operation through a clean, secure RESTful API.

The system is built around **8 independent business modules**, each handling a specific domain of the business — from authentication and product management to revenue analytics and complaint resolution.

> Built with a **security-first mindset**, the API uses JWT stateless authentication, role-based access control, and Redis-backed token blacklisting to ensure every endpoint is protected.

---
