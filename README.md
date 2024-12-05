# Bank Management System

A comprehensive **Bank Management System** developed using **Spring Boot**. This project demonstrates the implementation of core banking functionalities like account creation, transaction management, user authentication, and more, using Spring Boot features such as **Spring Security**, **JPA**, and **RESTful APIs**.

---

## Table of Contents

- [Features](#features)  
- [Tech Stack](#tech-stack)  
- [Setup Instructions](#setup-instructions)  
- [API Documentation](#api-documentation)  
- [Postman Collection](#postman-collection)
  
---

## Features

- **User Authentication**: Login/Signup secured with **Spring Security**.  
- **Account Management**: View, create, and delete bank accounts.  
- **Transaction Management**: Deposit, withdraw, and transfer funds between accounts.  
- **Role-based Access Control**: Features are role-specific for Admins and Customers.  
- **RESTful API Design**: Easy integration with other systems.  

---

## Tech Stack

- **Backend Framework**: Spring Boot  
- **Database**: MySQL  
- **Security**: Spring Security (JWT-based authentication)  
- **Build Tool**: Maven  
- **API Testing**: Postman  

---

## Setup Instructions

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-repository/bank-management-system.git
   ```
2. Navigate to the project directory:  
   ```bash
   cd bank-management-system
   ```
3. Configure the database in `application.properties`:  
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/your_database
   spring.datasource.username=your_username
   spring.datasource.password=your_password
   ```
4. Run the application:  
   ```bash
   mvn spring-boot:run
   ```
5. Access the application at `http://localhost:8080`.

---

## API Documentation

The API endpoints provided by this system are as follows:

| HTTP Method | Endpoint          | Description              | Authentication Required |
|-------------|-------------------|--------------------------|--------------------------|
| GET         | /accounts         | Fetch all accounts       | Yes                      |
| POST        | /accounts         | Create a new account     | Yes                      |
| PUT         | /accounts/{id}    | Update account details   | Yes                      |
| DELETE      | /accounts/{id}    | Delete an account        | Yes                      |
| POST        | /transactions     | Perform a transaction    | Yes                      |

> For a complete list of endpoints, refer to the [Postman Collection](#postman-collection).

---

## Postman Collection

You can access and test the APIs using the Postman collection linked below:  

https://hello4-6853.postman.co/workspace/hello-Workspace~72ac151c-2736-4e93-9823-40b66a270ada/collection/30485759-f5b3fa8c-bda3-4269-83f2-d00f1f961d3d?action=share&creator=30485759

1. Open the URL in your browser.  
2. Import the collection into Postman.  
3. Configure the required environment variables if necessary (e.g., `BASE_URL`, `TOKEN`).  

