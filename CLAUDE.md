# claude-java-app

A Spring Boot application with Gradle build system.

## Project Structure

```
src/
├── main/
│   ├── java/com/example/app/   # Java source files
│   │   └── ClaudeJavaAppApplication.java
│   └── resources/
│       └── application.properties
└── test/
    └── java/com/example/app/
        └── ClaudeJavaAppApplicationTests.java
```

## Build System

**Gradle** with Spring Boot plugin

- Spring Boot: 3.4.4
- Java: 17
- Dependency Management: io.spring.dependency-management 1.1.7

## Dependencies

- `spring-boot-starter-web` - Web application support
- `spring-boot-starter-actuator` - Production monitoring endpoints
- `spring-boot-devtools` - Development-time tools (dev only)
- `spring-boot-starter-test` - Testing with JUnit 5

## Commands

```bash
# Run the application
./gradlew bootRun

# Build the project
./gradlew build

# Run tests
./gradlew test

# Clean build
./gradlew clean build
```

## Configuration

Edit `src/main/resources/application.properties`:
- `server.port=8080` (default)
- Actuator endpoints: `/actuator/health`, `/actuator/info`

## Development Guidelines

- Package: `com.example.app`
- Testing: JUnit 5 with Spring Boot Test
- Main class: `ClaudeJavaAppApplication`
