# 🎬 Movie Ticket Booking System

A backend-focused **Movie Ticket Booking System** developed using **Java and Spring Boot**. The application provides REST APIs for managing movies, shows, theatres, seats, and ticket bookings, with persistent data storage using MySQL.

The project follows a layered backend architecture using **Controller, Service, Repository, and Entity** components.

---

## 🚀 Features

* 🎥 Movie management
* 🎭 Theatre and show management
* 💺 Seat management and availability
* 🎟️ Movie ticket booking
* 👤 User management
* 🔄 Booking and cancellation workflow
* 🗄️ MySQL database integration
* 🌐 RESTful APIs
* ✅ Request validation
* ⚠️ Exception handling
* 📦 Maven-based dependency management
* 🏗️ Layered Spring Boot architecture

---

## 🛠️ Technology Stack

| Technology      | Usage                           |
| --------------- | ------------------------------- |
| Java 17+        | Backend development             |
| Spring Boot     | Application framework           |
| Spring Data JPA | Database access                 |
| Hibernate       | ORM                             |
| MySQL           | Relational database             |
| REST API        | Client-server communication     |
| Maven           | Build and dependency management |
| Git & GitHub    | Version control                 |

---

## 🏗️ Project Architecture

The application follows a layered architecture:

```text
Client
   │
   ▼
Controller Layer
   │
   ▼
Service Layer
   │
   ▼
Repository Layer
   │
   ▼
MySQL Database
```

### Main Components

```text
src/main/java
│
├── controller
│   └── REST API endpoints
│
├── service
│   └── Business logic
│
├── repository
│   └── Database operations
│
├── entity
│   └── JPA entities
│
└── configuration
    └── Application configuration
```

---

## 📋 Prerequisites

Before running the project, make sure you have:

* Java 17 or later
* Maven
* MySQL Server
* Git
* IDE such as IntelliJ IDEA, Eclipse, or Spring Tool Suite

Verify Java installation:

```bash
java -version
```

Verify Maven installation:

```bash
mvn -version
```

---

## ⚙️ Database Configuration

Create a MySQL database:

```sql
CREATE DATABASE movie_ticket_booking;
```

Update the database configuration in:

```text
src/main/resources/application.properties
```

Example:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/movie_ticket_booking
spring.datasource.username=root
spring.datasource.password=YOUR_PASSWORD

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
```

Replace `YOUR_PASSWORD` with your local MySQL password.

> Do not commit real database passwords or other credentials to GitHub.

---

## ▶️ Running the Application

### 1. Clone the repository

```bash
git clone https://github.com/naman-1624/MovieTicketBookingSystem.git
```

### 2. Navigate to the project

```bash
cd MovieTicketBookingSystem
```

### 3. Build the project

```bash
mvn clean install
```

### 4. Run the application

```bash
mvn spring-boot:run
```

The application will start on:

```text
http://localhost:8080
```

---

## 🔌 API Overview

The application exposes REST APIs for different modules.

| Module   | Operations                   |
| -------- | ---------------------------- |
| Movies   | Create, Read, Update, Delete |
| Shows    | Create, Read, Update, Delete |
| Theatres | Create, Read, Update, Delete |
| Seats    | Availability and management  |
| Bookings | Create, View, Cancel         |
| Users    | User management              |

> API endpoints may vary depending on the implementation in the current version of the project.

---

## 🗂️ Database

The application uses **MySQL** for persistent storage.

The database manages information related to:

* Users
* Movies
* Theatres
* Shows
* Seats
* Bookings

JPA/Hibernate is used to map Java entities to relational database tables.

---

## 🧪 Testing

To run the available tests:

```bash
mvn test
```

---

## 🔮 Future Improvements

Possible improvements include:

* JWT-based authentication and authorization
* Role-based access control
* Payment gateway integration
* Real-time seat locking
* Booking confirmation through email
* Redis-based seat availability caching
* Swagger/OpenAPI documentation
* Docker containerization
* Unit and integration test coverage
* Frontend integration

---

## 📌 Project Purpose

This project is intended for learning and demonstrating backend development concepts using **Java, Spring Boot, REST APIs, JPA, Hibernate, and MySQL**.

It provides practical experience with:

* Object-Oriented Programming
* Spring Boot application development
* REST API design
* Database integration
* JPA entity relationships
* CRUD operations
* Business logic implementation
* Layered architecture
* Exception handling
* Maven
* Git and GitHub

---

## 👨‍💻 Development & Attribution

This repository is a working/extended version of a movie-ticket-booking application originally available from **JavaaTechSolutions**.

Original repository:

https://github.com/JavaaTechSolutions/movie-ticket-booking-system

The original contributors are acknowledged for the base project. This repository is maintained separately for learning, development, and further enhancements.

Any modifications or additional implementations in this repository should be clearly attributed to their respective contributors.

---

## 📄 License

The original repository does not appear to include an explicit open-source license.

This repository therefore does not grant additional rights to the original code beyond any rights provided by the original author(s). Please refer to the original repository and obtain appropriate permission before redistributing or commercially using the original code.

---

## ⭐ If You Find This Project Useful

Feel free to explore the project, study the implementation, and use it as a reference for learning Java and Spring Boot backend development.
