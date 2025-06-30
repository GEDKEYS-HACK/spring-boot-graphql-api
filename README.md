# Spring Boot GraphQL API 🚀

![GitHub release](https://img.shields.io/github/release/GEDKEYS-HACK/spring-boot-graphql-api.svg) ![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Java Version](https://img.shields.io/badge/java-11-orange.svg)

Welcome to the **Spring Boot GraphQL API** repository! This project serves as a modern, scalable, and secure backend API template built with Spring Boot and GraphQL. It demonstrates best practices for maintainable, extensible, and production-ready backend development.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [API Endpoints](#api-endpoints)
- [Authentication](#authentication)
- [Testing](#testing)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)
- [Links](#links)

## Features

- **GraphQL API**: Provides a flexible and efficient way to query and manipulate data.
- **Layered Architecture**: Organizes code into layers for better maintainability.
- **JWT Authentication**: Secure your API with JSON Web Tokens.
- **Microservices Ready**: Easily deployable as a microservice.
- **Production-Ready**: Follows best practices for a stable and secure deployment.

## Technologies Used

- **Spring Boot**: A powerful framework for building Java applications.
- **GraphQL**: A query language for APIs.
- **Gradle**: A build automation tool for Java projects.
- **Java**: The programming language used for development.
- **JWT**: For secure authentication.
- **PostgreSQL**: Database for data storage.
- **Docker**: For containerization and deployment.

## Getting Started

To get started with this project, clone the repository and run the following commands:

```bash
git clone https://github.com/GEDKEYS-HACK/spring-boot-graphql-api.git
cd spring-boot-graphql-api
./gradlew bootRun
```

You can also download the latest release from the [Releases section](https://github.com/GEDKEYS-HACK/spring-boot-graphql-api/releases) and execute it.

## Project Structure

The project follows a layered architecture. Here’s a brief overview of the structure:

```
spring-boot-graphql-api/
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── example/
│   │   │           └── graphqlapi/
│   │   │               ├── controller/
│   │   │               ├── service/
│   │   │               ├── repository/
│   │   │               └── model/
│   │   └── resources/
│   │       └── application.yml
│   └── test/
│       └── java/
└── build.gradle
```

- **controller/**: Contains the API endpoints.
- **service/**: Business logic goes here.
- **repository/**: Data access layer.
- **model/**: Data models and entities.

## API Endpoints

This API exposes several endpoints. Here are some examples:

- **Get All Items**
  - **Query**: `query { items { id name } }`
  
- **Create Item**
  - **Mutation**: `mutation { createItem(name: "New Item") { id name } }`

Refer to the [GraphQL documentation](https://graphql.org/learn/) for more details on how to structure queries and mutations.

## Authentication

This API uses JWT for authentication. To access protected endpoints, include the JWT in the `Authorization` header as follows:

```
Authorization: Bearer <your_token>
```

To obtain a token, send a POST request to the login endpoint with your credentials.

## Testing

Unit tests are included in the `src/test/java` directory. You can run the tests using:

```bash
./gradlew test
```

This will execute all tests and provide you with a report.

## Deployment

You can deploy this application using Docker. Here’s how to build the Docker image:

```bash
docker build -t spring-boot-graphql-api .
```

Then run the container:

```bash
docker run -p 8080:8080 spring-boot-graphql-api
```

This will expose the API on port 8080.

## Contributing

We welcome contributions! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Links

For more information, check the [Releases section](https://github.com/GEDKEYS-HACK/spring-boot-graphql-api/releases). 

Feel free to explore the code, suggest improvements, or raise issues. Your feedback is valuable!