# Banking Application (Spring Boot + PostgreSQL)

A simple **Banking REST API** built using **Spring Boot**, **Spring Data JPA**, and **PostgreSQL**.  
This project demonstrates a clean layered backend architecture with full CRUD operations, database persistence, and RESTful endpoints.

---

## 🚀 Features

- Create bank accounts
- Get all accounts
- Get account by ID
- Deposit money into an account
- Withdraw money from an account
- Delete an account
- Persistent data storage using PostgreSQL

---

## 🛠 Tech Stack

- **Java 21**
- **Spring Boot**
- **Spring Data JPA (Hibernate)**
- **PostgreSQL**
- **Maven**
- **REST APIs**

---

## 📁 Project Structure
src/main/java/com/banking_app
│
├── controller # REST controllers
├── service # Business logic
├── repository # JPA repositories
├── entity # JPA entities
├── dto # Data Transfer Objects
├── mapper # Entity ↔ DTO mapping
└── BankingAppApplication.java

Database Setup
1️⃣ Start PostgreSQL
Make sure PostgreSQL is running on port 5440.
2️⃣ Create the database
psql -U postgres -p 5440
CREATE DATABASE banking_app;
## Adding Test Data (PostgreSQL)
INSERT INTO accounts (account_holder_name, balence)
VALUES ('John Doe', 1000);

INSERT INTO accounts (account_holder_name, balence)
VALUES ('Jane Smith', 2500);
## Example tests 
GET all accounts
Open your browser and go to:
http://localhost:8080/api/accounts
GET account by ID
http://localhost:8080/api/accounts/1

Note: if you have Postman, it would be better to use that since you can insert data directly into your database instead of running SQL commands on your terminal
