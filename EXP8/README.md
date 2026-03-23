# 📘 EXP8 – Student CRUD REST Service (Spring Boot)

This project demonstrates the development of a RESTful backend service using **Spring Boot** and **Hibernate (JPA)** to perform CRUD operations on student data stored in a MySQL database.

---

## 🧩 Overview

The application exposes a set of REST endpoints that allow interaction with student records. It supports full lifecycle operations including creation, retrieval, modification, and deletion of data.

---

## ⚙️ Technology Stack

* Java (JDK 21)
* Spring Boot Framework
* Spring Web (REST APIs)
* Spring Data JPA (Hibernate ORM)
* MySQL Database
* Maven (Build Tool)

---

## 📁 Directory Structure

```
try/
 └── src/
      └── main/
           ├── java/
           │     └── com.example.demo
           │           ├── controller
           │           ├── service
           │           ├── repository
           │           └── model
           │
           └── resources/
                 └── application.properties
```

---

## 🔗 Base Endpoint

```
http://localhost:8080/api/students
```

---

## 📡 Available API Routes

| HTTP Method | Endpoint           | Purpose                      |
| ----------- | ------------------ | ---------------------------- |
| GET         | /api/students      | Retrieve all student records |
| GET         | /api/students/{id} | Retrieve a specific student  |
| POST        | /api/students      | Insert a new student         |
| PUT         | /api/students/{id} | Modify existing student      |
| DELETE      | /api/students/{id} | Remove student record        |

---

## 🗄️ Database Setup

1. Create a MySQL database:

```sql
CREATE DATABASE student_management;
```

2. Configure credentials in:

```
src/main/resources/application.properties
```

---

## ▶️ Running the Application

Navigate to the `try` directory and execute:

### Windows

```
mvnw.cmd spring-boot:run
```

### macOS/Linux

```
./mvnw spring-boot:run
```

The server will start on:

```
http://localhost:8080
```

---

## 🔄 Working Mechanism

* Incoming HTTP requests are handled by **Controller classes**
* Business logic is processed in the **Service layer**
* Data persistence is managed via **Repository interfaces**
* Hibernate maps Java objects to database tables

---

## 🎯 Learning Highlights

* Building REST APIs with Spring Boot
* Integrating Hibernate for ORM
* Performing CRUD operations
* Structuring backend applications using layered architecture

---

## 👤 Developed By

Riyan Imtiyaz
