# Spring Boot REST API Fundamentals

A foundational Java and Spring Boot REST API project focused on HTTP CRUD endpoints, in-memory data management, controller structure, property configuration, and embedded server setup.

The project simulates a simple animal management API using Spring Boot and an in-memory `Map` structure.

## Overview

This project demonstrates the fundamentals of building a REST API with Spring Boot.

The application manages animal records through basic CRUD endpoints and stores data in memory using a `Map<Integer, Animal>` structure.

The main focus is REST controller design, HTTP request handling, application configuration, `@Value` property injection, embedded server configuration, and JSON-based API responses.

## Tech Stack

* Java
* Spring Boot
* Spring Web
* Maven
* REST API
* In-memory data storage
* Java Map
* `@Value` property injection
* Spring DevTools
* Embedded server configuration

## Core Concepts

* Spring Boot project structure
* REST controller creation
* HTTP CRUD endpoint design
* In-memory data management with `Map`
* JSON response handling
* Request body handling
* Path variable usage
* Application property configuration
* `@Value` annotation usage
* Embedded server port configuration
* Spring DevTools auto-restart behavior

## Domain Model

### Animal

The `Animal` model represents a simple animal record.

Main fields:

* `id`
* `name`

## Features

* Get all animals
* Get animal by ID
* Create a new animal
* Update an existing animal
* Delete an animal
* In-memory storage with `Map<Integer, Animal>`
* Custom application properties
* Server port configuration
* JSON-based REST responses
* Simple controller and entity package structure

## Main API Endpoints

| Method | Endpoint                  | Description         |
| ------ | ------------------------- | ------------------- |
| GET    | `/workintech/animal`      | Get all animals     |
| GET    | `/workintech/animal/{id}` | Get animal by ID    |
| POST   | `/workintech/animal`      | Create a new animal |
| PUT    | `/workintech/animal/{id}` | Update animal by ID |
| DELETE | `/workintech/animal/{id}` | Delete animal by ID |

## Backend Architecture

The project follows a simple Spring Boot REST API structure:

```text
Controller Layer
↓
In-Memory Map Storage
↓
Entity Model
↓
Application Configuration
```

This structure keeps request handling, temporary data storage, domain modeling, and configuration separated.

## Project Structure

```text
src/
 └── main/
     ├── java/
     │   └── com/workintech/fsswebs17d1/
     │       ├── controller/
     │       │   └── AnimalController.java
     │       └── entity/
     │           └── Animal.java
     └── resources/
         └── application.properties
```

## Application Properties

The project uses custom values from `application.properties`, such as:

```properties
course.name=Spring Boot
project.developer.fullname=Your Name
server.port=8585
```

These values can be accessed inside the application using the `@Value` annotation.

## What This Project Demonstrates

* Creating a Spring Boot REST API
* Building CRUD endpoints
* Managing temporary data with an in-memory map
* Using path variables and request bodies
* Returning JSON responses
* Organizing controller and entity packages
* Reading custom values from `application.properties`
* Configuring the server port
* Using Spring DevTools during development

## Getting Started

### Prerequisites

Make sure you have the following installed:

* Java 17+
* Maven
* IntelliJ IDEA or another Java IDE

### Installation

Clone the repository:

```bash
git clone https://github.com/emreyildirim-33/spring-boot-rest-api-fundamentals.git
cd spring-boot-rest-api-fundamentals
```

Run the project:

```bash
./mvnw spring-boot:run
```

The application runs locally at:

```text
http://localhost:8585
```

## API Testing

You can test the endpoints using:

* Postman
* IntelliJ HTTP Client
* Browser for simple GET requests

## Notes

This project focuses on Spring Boot REST API fundamentals, CRUD endpoint design, in-memory data handling, controller structure, property configuration, and embedded server setup.

The main purpose is to demonstrate the foundation of building REST APIs with Spring Boot before moving into database-backed persistence and more advanced backend architecture.

## Repository

GitHub: https://github.com/emreyildirim-33/spring-boot-rest-api-fundamentals
