Car Rental System

Overview

The Car Rental System is a web-based application designed to facilitate car rentals for users and provide management tools for administrators. The system is developed using Java with the Spring Boot framework, Hibernate ORM, and MySQL database. The project includes two main modules: the Admin module and the User module.

Features

User Module

Browse Cars: View available cars for rent.

Search Cars: Search for cars based on criteria such as model, type, and availability.

Book Cars: Rent a car by selecting the desired vehicle and rental period.

User Registration and Login: Create a new account or log in to an existing account.

View Booking History: Check previous and upcoming bookings.

Admin Module

Add Cars: Add new cars to the inventory.

Update Car Details: Edit details of existing cars (e.g., price, availability, specifications).

Delete Cars: Remove cars from the inventory.

View Bookings: Access and manage all user bookings.

Generate Reports: View reports for car usage and revenue.

Technology Stack

Backend: Java, Spring Boot

Database: MySQL

ORM: Hibernate

Frontend: Angular (optional, depending on integration)

Build Tool: Maven

Prerequisites

Java 17 or later

Maven 3.8+

MySQL 8.0+

IDE: IntelliJ IDEA, Eclipse, or any preferred Java IDE

Setup and Installation

Step 1: Clone the Repository

git clone https://github.com/your-repository-url/car-rental-system.git
cd car-rental-system

Step 2: Configure the Database

Create a MySQL database named car_rental.

Update the application.properties file in the src/main/resources directory with your database credentials:

spring.datasource.url=jdbc:mysql://localhost:3306/car_rental
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update

Step 3: Build and Run the Project

Build the project using Maven:

mvn clean install

Run the Spring Boot application:

mvn spring-boot:run

API Endpoints

User Endpoints

GET /api/cars: Get a list of available cars.

POST /api/bookings: Book a car.

GET /api/bookings/user/{userId}: Get a user's booking history.

Admin Endpoints

POST /api/admin/cars: Add a new car.

PUT /api/admin/cars/{carId}: Update car details.

DELETE /api/admin/cars/{carId}: Delete a car.

GET /api/admin/bookings: View all bookings.

Folder Structure

src
 ├── main
 │   ├── java
 │   │   ├── com.example.carrental
 │   │       ├── controller
 │   │       ├── service
 │   │       ├── repository
 │   │       ├── model
 │   │       └── dto
 │   ├── resources
 │       ├── application.properties
 │       └── static
 │
 ├── test
     └── java
         └── com.example.carrental

Future Enhancements

Integration with a payment gateway for online payments.

Advanced search filters (e.g., price range, car features).

Mobile app support.

Multi-language support.

License

This project is licensed under the MIT License. See the LICENSE file for details.

Contributors

Your Name

Feel free to fork this project and contribute by submitting a pull request.

