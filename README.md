# The Ultimate Reviewer

This is a **prototype backend** for a social media-like application focused on handling user authentication, image uploading, commenting, and user search capabilities using a **microservices** architecture.

---

## 🧠 Technologies Used

- Java 21
- Spring Boot
- Spring WebFlux
- Spring Cloud / Eureka Server
- Spring Security + JWT
- PostgreSQL
- RabbitMQ
- Cloudinary (image hosting)
- Docker / Docker Compose

---

## 🧩 Microservices

This project is split into several microservices:

| Microservice       | Description                                  | Port |
|--------------------|----------------------------------------------|------|
| `eureka-server`    | Service Discovery                             | 8761 |
| `api-gateway`      | Entry point, handles routing/auth             | 8080 |
| `user-service`     | Handles user registration, login, profile     | 8081 |
| `image-service`    | Uploads and fetches images (Cloudinary)       | 8082 |
| `comment-service`  | Manages comments on images                    | 8083 |
| `search-service`   | Handles search for users                      | 8084 |
| `notification-service` | Handles email notifications (future work) | 8085 |

---

## 🧪 Functionalities

- User registration and login with JWT authentication.
- Upload images using Cloudinary.
- View user profiles and their uploaded images.
- Add comments to images.
- Search for users.
- Service-to-service communication with RabbitMQ.
- Load balancing and routing via API Gateway.

---

## 🚀 How to Run

### Prerequisites

- Make sure **Docker** and **Docker Compose** are installed.

### Steps

1. Clone this repository:
   ```bash
   git clone https://github.com/your-org/theUltimateReviewer-central.git
   cd theUltimateReviewer-central
   ```

2. Build and run using Docker Compose:
   ```bash
   docker-compose up --build
   ```

3. The services will be available at their respective ports. You can modify the ports in the `docker-compose.yml` file if needed.

---

## 📁 Structure of this Repository

This repository contains links to all the associated microservices:

- [eureka-server](https://github.com/your-org/eureka-server)
- [api-gateway](https://github.com/your-org/api-gateway)
- [user-service](https://github.com/your-org/user-service)
- [image-service](https://github.com/your-org/image-service)
- [comment-service](https://github.com/your-org/comment-service)
- [search-service](https://github.com/your-org/search-service)
- [notification-service](https://github.com/your-org/notification-service)

> Each of the above repositories contains its own README with detailed instructions for running the service individually.

---

## 📌 Notes

- This project is still under development.
- It's designed primarily as a **backend prototype** for a potential social media-like application.
- The frontend is not included.
- Most refined parts: **user authentication**, **profile management**, **image upload**, and **routing**.

---

## 👨‍💻 Author

Made with ❤️ by [Your Name](https://github.com/your-github).

---

## 📝 License

This project is licensed under the MIT License.
