# StaySphere - Spring Boot Backend API

This is the Java Spring Boot backend service for **StaySphere**, a premium luxury hotel booking platform.

## 🛠️ Tech Stack
* **Framework**: Spring Boot 3.3.0, Java 17+
* **Database**: MongoDB (Spring Data MongoDB)
* **Build Tool**: Apache Maven 3.9.6
* **AI Integration**: Spring AI (OpenAI API integration for AI Travel Agent)
* **API Docs**: Springdoc OpenAPI / Swagger UI
* **Security**: JWT-based Authentication & Spring Security

---

## 🚀 Environment Variables
The application reads the following variables from the environment (default fallbacks are defined in `src/main/resources/application.yml`):
* `MONGODB_URI`: MongoDB Atlas connection URI.
* `JWT_SECRET`: Secret key for JWT generation.
* `CLIENT_URL`: Cross-Origin Resource Sharing (CORS) allowed origin for the frontend (defaults to `http://localhost:5173`).
* `SPRING_AI_OPENAI_API_KEY`: API Key for the AI Travel Agent functionality.

---

## ⚡ Setup & Run

### 1. Build and Run
Execute the Maven runner:
```bash
# If using the bundled Maven tool:
..\tools\apache-maven-3.9.6\bin\mvn spring-boot:run

# If Maven is installed globally on your path:
mvn spring-boot:run
```

The server runs on **port 8080** by default.

### 2. Swagger API Documentation
Once the server is running, you can explore the API endpoints interactively at:
👉 **[http://localhost:8080/swagger-ui/index.html](http://localhost:8080/swagger-ui/index.html)**
