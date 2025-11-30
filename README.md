# 🍽️ Surplus Food Redistribution System

A Java Swing + JDBC Desktop Application


A complete desktop-based Java application designed to reduce food wastage by connecting Donors, NGOs, and Admins on a single platform. Donors can upload surplus food details, NGOs can request food pickups, and Admins can monitor the entire process.

This project uses Java Swing for UI, JDBC for database connectivity, and MySQL for data storage, following OOP principles and modular architecture.

## 🚀 Features
🔹 Common Features

Secure login system (Donor, NGO, Admin)

User authentication using MySQL database

Interactive Java Swing-based UI

MVC-like layered architecture (UI → Logic → DB)

👤 Donor Module

Add surplus food details

View all posted donations

Track status: Available / Requested / Picked-up

Receive NGO pickup requests

Manage personal profile

🏢 NGO Module

View all available food donations

Request for specific donation pickup

Track request status: Pending / Approved / Completed

Update delivery/collection status

🛡️ Admin Module

Manage donors and NGOs

Approve/Reject user registrations

View all donations & requests

Generate system reports

Monitor system activity

## 🏗️ Project Architecture
1️⃣ Presentation Layer (UI)

Built using Java Swing
Includes:

Login Page

Registration Page

Donor Dashboard

NGO Dashboard

Admin Dashboard

Forms (Add Donation, View Requests, Manage Users etc.)

Swing components used:
JFrame, JPanel, JTable, JButton, JLabel, JTextField, JPasswordField, JScrollPane, etc.

2️⃣ Business Logic Layer (OOP Java Classes)

Core classes include:

Class	Purpose
User	Base class for all users
Donor	Inherits User, donor-specific features
NGO	Inherits User, NGO-specific features
Admin	Inherits User, admin functions
FoodDonation	Represents donation items
DonationRequest	Stores pickup requests
DatabaseConnection	JDBC connection manager

OOP Concepts Used:

Encapsulation (getters/setters)

Inheritance (User → Donor/NGO/Admin)

Polymorphism (login/roles)

Abstraction (interfaces for user operations)

3️⃣ Database Layer (MySQL + JDBC)

MySQL tables:

users
donations
requests
notifications


JDBC operations used:

Driver loading

Connection establishment

Prepared statements

Insert, Update, Delete, Select queries

ResultSet handling

Connection example:

Class.forName("com.mysql.cj.jdbc.Driver");
Connection con = DriverManager.getConnection(
      "jdbc:mysql://localhost:3306/surplus_food", "root", ""
);

## 🗄️ Database Schema (Sample)
users
id INT PRIMARY KEY
name VARCHAR(100)
email VARCHAR(100)
password VARCHAR(100)
role VARCHAR(20)  // donor, ngo, admin
address TEXT
phone VARCHAR(15)

donations
donation_id INT PRIMARY KEY
donor_id INT (FK)
food_type VARCHAR(100)
quantity VARCHAR(50)
expiry_date DATE
location TEXT
status VARCHAR(20)

requests
request_id INT PRIMARY KEY
donation_id INT (FK)
ngo_id INT (FK)
status VARCHAR(20)

## 🛠️ Technologies Used
Component	Technology
Programming Language	Java (Core Java, OOP)
UI	Java Swing
Database	MySQL
Connectivity	JDBC
Architecture	MVC-like, OOP-based
IDE	IntelliJ / Eclipse / NetBeans (any)**
Driver	mysql-connector-j.jar
## 📂 Folder Structure
Surplus-Food-Redistribution-System/
│── src/
│   ├── ui/ (Swing UI Forms)
│   ├── model/ (OOP classes)
│   ├── dao/ (JDBC database operations)
│   ├── service/ (Business logic)
│── database/
│   ├── surplus_food.sql
│── lib/
│   ├── mysql-connector-j.jar
│── README.md

## ▶️ How to Run the Project
1️⃣ Install Requirements

JDK 8+

MySQL Server

MySQL Workbench / phpMyAdmin

mysql-connector-java.jar

2️⃣ Import Database

Open MySQL

Create database:

CREATE DATABASE surplus_food;


Import the surplus_food.sql file

3️⃣ Set JDBC Credentials

In DatabaseConnection.java:

String url = "jdbc:mysql://localhost:3306/surplus_food";
String username = "root";
String password = "";

4️⃣ Add MySQL Connector JAR

Add mysql-connector-j.jar to your project classpath.

5️⃣ Run Main File

Open IDE

Run Main.java

Login screen will appear

## 🧪 Screenshots (Optional Section)

(Add here when available)

## 📌 Future Enhancements

Email/OTP authentication

Google Maps API for actual distance-based matching

Push notifications

Analytics dashboard

REST API / Web version

## 🤝 Contributors

Prathamesh Bansode

Team members (add names)

## 📜 License

This project is open-source and available for academic use.

## ⭐ If you like this project

Don’t forget to ⭐ star the repo on GitHub!
