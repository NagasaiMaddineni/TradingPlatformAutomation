# FinTrade

FinTrade is a learning project for building a paper-trading application and its end-to-end test automation framework. It is developed in small steps; this first milestone is only the Spring Boot application foundation and health check.

## Prerequisites

- Java Development Kit (JDK) 21
- Apache Maven 3.9 or newer

Verify the tools are available in a terminal:

```powershell
java -version
mvn -version
```

## Run the application

From the project root:

```powershell
mvn spring-boot:run
```

When startup completes, check the health endpoint at `http://localhost:8080/actuator/health`. It should return JSON with status `UP`.

## Run the test

```powershell
mvn test
```

The current test starts the Spring application in a test environment and checks the health endpoint. PostgreSQL, Kafka, Alpaca, and the web UI are future milestones and are not configured yet.