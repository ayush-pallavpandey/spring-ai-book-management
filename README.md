# 📚 Spring AI Book Management System

<div align="center">

![Java](https://img.shields.io/badge/Java-21-orange?style=for-the-badge&logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.x-6DB33F?style=for-the-badge&logo=springboot)
![Spring AI](https://img.shields.io/badge/Spring_AI-Latest-blue?style=for-the-badge)
![Spring Security](https://img.shields.io/badge/Spring_Security-JWT-success?style=for-the-badge)
![MySQL](https://img.shields.io/badge/MySQL-Database-blue?style=for-the-badge&logo=mysql)
![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?style=for-the-badge&logo=docker)
![Swagger](https://img.shields.io/badge/Swagger-OpenAPI-green?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

**An AI-powered Book Management System built with Spring Boot, Spring AI, JWT Authentication, MySQL, and Docker.**

*Designed using production-ready backend architecture with intelligent book recommendations, semantic search, and secure REST APIs.*

</div>

---

# 🚀 Project Overview

The **Spring AI Book Management System** is a modern backend application that combines traditional Library Management features with **Artificial Intelligence**.

Users can securely manage books while using AI-powered capabilities such as:

- 🤖 Natural language book search
- 📖 AI-generated book recommendations
- ✨ Smart summaries
- 🏷️ Automatic category suggestions
- 💬 Conversational book assistant

This project demonstrates how **Spring AI** can be integrated into enterprise-grade Spring Boot applications.

---

# ❓ What problem does this solve?

Traditional Library Management Systems rely on keyword-based search and manual categorization, making it difficult for users to discover relevant books.

This project solves several real-world challenges:

- Difficult book discovery
- Poor recommendation systems
- Manual category management
- Time-consuming searches
- Lack of intelligent interaction
- Limited user engagement

Instead of searching by exact title, users can ask:

> "Recommend beginner Java books"

or

> "Books similar to Clean Code"

The AI understands intent and returns meaningful results.

---

# 💡 Why did I build this?

I wanted to combine **Java Backend Development** with **Generative AI** to demonstrate how modern enterprise applications can become smarter using Large Language Models.

The project helped me learn:

- Spring AI integration
- Prompt Engineering
- REST API development
- Secure authentication using JWT
- Layered Architecture
- Docker containerization
- Clean Code practices
- Production-ready backend development

This repository is part of my learning journey toward becoming a **Java Backend Engineer specializing in AI-powered applications**.

---

# ⭐ Key Features

## User Features

- User Registration
- Secure Login
- JWT Authentication
- Role-Based Authorization
- View Books
- Search Books
- Borrow Books
- Return Books
- View Borrow History

---

## Admin Features

- Add Books
- Update Books
- Delete Books
- Manage Users
- Manage Inventory
- Dashboard APIs

---

## AI Features

- AI Book Recommendations
- Natural Language Search
- Book Summary Generation
- Category Prediction
- Reading Suggestions
- AI Chat Assistant
- Similar Book Suggestions

---

# 🛠 Technology Stack

| Category | Technologies |
|-----------|--------------|
| Language | Java 21 |
| Framework | Spring Boot 3 |
| AI | Spring AI |
| Security | Spring Security + JWT |
| ORM | Spring Data JPA + Hibernate |
| Database | MySQL |
| API | REST API |
| Documentation | Swagger / OpenAPI |
| Testing | JUnit 5, Mockito |
| Build Tool | Maven |
| Containerization | Docker |
| Version Control | Git & GitHub |
| CI/CD | GitHub Actions |
| Cloud (Planned) | AWS EC2 |

---

# 🏛 Architecture

```
                    Client
                       │
            REST API Requests
                       │
         Spring Security (JWT)
                       │
               REST Controllers
                       │
              Service Layer
                       │
      ┌─────────────────────────┐
      │                         │
Business Logic           Spring AI Service
      │                         │
Repository Layer        AI Model / LLM
      │
     MySQL Database
```

Architecture follows:

- Layered Architecture
- RESTful API Design
- Repository Pattern
- Dependency Injection
- SOLID Principles
- Clean Code Practices

---

# 📂 Project Structure

```
spring-ai-book-management
│
├── src
│   ├── main
│   │   ├── java
│   │   │   ├── controller
│   │   │   ├── service
│   │   │   ├── repository
│   │   │   ├── entity
│   │   │   ├── dto
│   │   │   ├── security
│   │   │   ├── config
│   │   │   ├── ai
│   │   │   ├── exception
│   │   │   └── util
│   │
│   └── resources
│
├── docs
│
├── docker
│
├── screenshots
│
├── README.md
│
└── pom.xml
```

---

# 🔐 Authentication

Authentication is implemented using:

- JWT Tokens
- Spring Security
- BCrypt Password Encoding
- Role-Based Access Control

Roles

- ADMIN
- USER

---

# 🤖 Spring AI Integration

The project integrates Spring AI to provide:

- Intelligent Recommendations
- Semantic Search
- AI Summaries
- Natural Language Queries
- Reading Assistant

Example Prompt

```
Recommend Java books for beginners.
```

Response

```
Effective Java

Head First Java

Java: The Complete Reference
```

---

# 📖 REST API Documentation

## Authentication

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | /api/auth/register | Register User |
| POST | /api/auth/login | Login |

---

## Books

| Method | Endpoint |
|---------|----------|
| GET | /api/books |
| GET | /api/books/{id} |
| POST | /api/books |
| PUT | /api/books/{id} |
| DELETE | /api/books/{id} |

---

## Borrow

| Method | Endpoint |
|---------|----------|
| POST | /api/borrow |
| POST | /api/return |
| GET | /api/history |

---

## AI APIs

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | /api/ai/recommend | AI Recommendations |
| POST | /api/ai/search | Natural Language Search |
| POST | /api/ai/summary | Generate Summary |
| POST | /api/ai/chat | Book Assistant |

---

# 📑 Swagger Documentation

After running the application:

```
http://localhost:8080/swagger-ui/index.html
```

Swagger provides:

- Interactive API Testing
- Request Validation
- Response Examples
- API Schemas

---

# ⚙️ How do I run it?

## Clone Repository

```bash
git clone https://github.com/yourusername/spring-ai-book-management.git
```

---

## Navigate

```bash
cd spring-ai-book-management
```

---

## Configure Database

Update

```
application.properties
```

```
spring.datasource.url=
spring.datasource.username=
spring.datasource.password=
```

---

## Configure AI API Key

```
spring.ai.openai.api-key=YOUR_API_KEY
```

---

## Run

Using Maven

```bash
mvn spring-boot:run
```

Or

```bash
mvn clean install
java -jar target/book-management.jar
```

---

## Run with Docker

```bash
docker-compose up --build
```

---

# 🧪 Running Tests

```bash
mvn test
```

Tests include:

- Unit Tests
- Service Tests
- Repository Tests
- Security Tests

---

# 📸 Screenshots

```
screenshots/

├── login.png
├── register.png
├── swagger-ui.png
├── ai-chat.png
├── recommendation.png
├── dashboard.png
```

---

# 🌟 Future Improvements

Planned enhancements include:

- Microservices Architecture
- Kubernetes Deployment
- AWS EC2 Deployment
- Redis Caching
- Elasticsearch Integration
- Vector Database Support
- RAG (Retrieval-Augmented Generation)
- Personalized Recommendation Engine
- Email Notifications
- Book Reviews & Ratings
- PDF Upload & AI Analysis
- OCR for Book Covers
- Analytics Dashboard
- CI/CD Pipeline
- Multi-language Support

---

# 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push your branch
5. Open a Pull Request

---

# 📄 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

**Ayush Pallav Pandey**

Java Backend Developer | Spring Boot Developer | AI Enthusiast

- 💼 Java Backend Development
- ☁️ AWS (Learning)
- 🤖 Spring AI
- 🐳 Docker
- 🔒 Spring Security
- 🚀 Building scalable backend applications

---

## ⭐ If you found this project useful, consider giving it a Star!
