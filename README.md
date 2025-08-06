# The Ultimate Reviewer – Central Documentation

**The Ultimate Reviewer** is a microservices-based backend system for managing image-based content, user profiles, comments, and more. It follows a distributed architecture using Spring Boot, Spring Cloud, and reactive programming with WebFlux.

> ⚠️ This repository does **not** contain executable code.  
> It serves as a central place for documentation, architecture overview, and service links.

---

## 🧱 Architecture Overview

The system is composed of several independent microservices, each responsible for a specific part of the functionality:

| **Service**         | **Description** |
|---------------------|-----------------|
| **Eureka Server**   | Service discovery server for registering and locating microservices. |
| **API Gateway**     | Gateway that routes external requests to the appropriate microservices using Spring Cloud Gateway. |
| **Post Service**    | Handles image posting. Uses the Cloudinary service to store and serve uploaded images. |
| **Cloudinary Service** | Dedicated service for managing images via the Cloudinary API. |
| **Profile Service** | Manages user profiles, including personal information, profile pictures, and settings. |
| **Review Auth Service** | Handles user registration, login, and JWT-based authentication. |
| **Database**        | Container with the database used by the microservices. |



Each service is a standalone project and can be found in this GitHub organization:  
🔗 [https://github.com/your-org-name](https://github.com/your-org-name)

---

## ▶️ How to Run the System

Each microservice must be cloned and run individually.  
Please refer to the `README.md` of each service repository for:

- Environment variable setup
- How to run it locally (using `mvn spring-boot:run`, Docker, or similar)
- Dependencies like MongoDB, Cloudinary, RabbitMQ, etc.

> ⚠️ A unified `docker-compose` setup for running all services together is not available (yet).

---

## 🌱 Project Status

This project is a prototype and proof-of-concept.  
It focuses primarily on backend architecture and communication between services, including:

- Stateless authentication using JWT
- Centralized gateway routing
- Reactive programming (WebFlux)
- Asynchronous messaging with RabbitMQ

---

## 📫 Contributing

Feel free to explore, clone, or extend the services.  
You can fork any repository under the organization and contribute improvements.

---

## 📎 Related Repositories

Here are direct links to the most important services (replace with real links):

- [User Service](https://github.com/your-org-name/user-service)
- [Image Service](https://github.com/your-org-name/image-service)
- [Comment Service](https://github.com/your-org-name/comment-service)
- [Search Service](https://github.com/your-org-name/search-service)
- [Gateway Service](https://github.com/your-org-name/gateway-service)
- [Eureka Server](https://github.com/your-org-name/eureka-server)

---

## 📘 License

This project is for educational purposes and internal experimentation.

---

