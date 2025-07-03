A full-stack Java Spring Boot application for managing personal journal entries, with integrated Google Authentication, Redis caching, and weather data enrichment.

## 🌟 Features

- 📓 Create, read, update, and delete journal entries
- 🔐 Secure authentication with Google OAuth2
- 🌦 Weather data integration for journal context
- 💾 Redis caching for performance
- 🔍 RESTful APIs with Swagger UI documentation
- 🛡 Spring Security-based access control
- 🧪 Unit and integration test structure

## 🛠 Tech Stack

- **Java 17+**
- **Spring Boot**
- **Spring Security**
- **Spring Data JPA**
- **MySQL / PostgreSQL (configurable)**
- **Redis**
- **Google OAuth2**
- **Swagger (SpringFox)**
- **Maven**

## 📦 Project Structure

```

.
├── .github/workflows        # CI/CD pipeline
├── .mvn/wrapper             # Maven wrapper
├── src/main/java
│   └── net/engineeringdigest/journalApp
│       ├── controller       # REST controllers
│       ├── config           # App and security configurations
│       ├── dto              # Data Transfer Objects
│       ├── entity           # JPA entities
│       ├── repository       # Spring Data repositories
│       ├── service          # Business logic
│       ├── constants        # Application constants
│       ├── cache            # Redis caching
│       └── api              # External API response models
└── pom.xml                  # Maven dependencies and build config

````

## 🚀 Getting Started

### Prerequisites

- Java 17+
- Maven 3.6+
- MySQL or PostgreSQL
- Redis server running locally or in Docker

### Clone the repo

```bash
git clone https://github.com/yourusername/journalApp.git
cd journalApp
````

### Set up environment variables

Create an `.env` or use `application.properties`/`application.yml` under `src/main/resources/`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/journal_app
spring.datasource.username=root
spring.datasource.password=yourpassword

spring.redis.host=localhost
spring.redis.port=6379

google.client.id=YOUR_GOOGLE_CLIENT_ID
google.client.secret=YOUR_GOOGLE_CLIENT_SECRET
```

### Run with Maven

```bash
./mvnw spring-boot:run
```

### Swagger API Docs

Once running, visit:

```
http://localhost:8080/swagger-ui/index.html
```

## 🧪 Running Tests

```bash
./mvnw test
```

## 📤 Deployment

This project includes a GitHub Actions workflow (`.github/workflows/build.yml`) for CI/CD. You can deploy to services like Heroku, AWS Elastic Beanstalk, or Docker.

## 👥 Contributing

Pull requests are welcome! For major changes, open an issue first to discuss what you would like to change.

## 📝 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## 👨‍💻 Author

Built by [Engineering Digest](https://engineeringdigest.in) and contributors.

