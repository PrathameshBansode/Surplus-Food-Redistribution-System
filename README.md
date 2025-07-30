# 🍱 Surplus Food Redistribution System

The **Surplus Food Redistribution System** is a web-based platform designed to bridge the gap between food donors and NGOs. It helps minimize food wastage by enabling surplus food from restaurants, events, or households to be redistributed efficiently to those in need through verified NGO partners.

---

## 🌟 Features

- 🍽️ **Food Donation Portal** for individuals or organizations
- 🏢 **NGO Dashboard** to manage and track food requests
- 🧑‍🤝‍🧑 **Role-based Login System** for Admin, Donor, and NGO users
- 📍 **Location-Based Matching** of donors and NGOs
- 📨 **Notification System** for new donations and pickup requests
- 📦 **Pickup & Delivery Management** with status tracking
- 📊 **Admin Panel** for system monitoring and user management

---

## 🧰 Tech Stack

| Category        | Tools / Frameworks                    |
|----------------|----------------------------------------|
| Frontend       | HTML, CSS, JavaScript, Bootstrap       |
| Backend        | PHP                                    |
| Database       | MySQL                                  |
| Server         | Apache (XAMPP/WAMP for local testing)  |
| Hosting (Optional) | GitHub Pages / Any PHP-compatible host |

---

## 📁 Project Structure

Surplus-Food-Redistribution-System/
├── assets/ # CSS, JS, and image files
├── includes/ # Reusable PHP includes (navbars, DB connections)
├── donor/ # Donor-specific pages
├── ngo/ # NGO-specific dashboard and functions
├── admin/ # Admin panel files
├── index.php # Home / Landing page
├── login.php # Login functionality
├── register.php # Registration forms
└── README.md


---
##  Set Up Environment
Install XAMPP or WAMP

Move the project folder to the htdocs/ directory (XAMPP)

Start Apache and MySQL from the XAMPP Control Panel

## Import Database
Open phpMyAdmin → Create a new database (e.g., surplus_food_db)

Import the .sql file located in the project (if provided)
## 🛠️ Getting Started (Local Setup)
## 🔐 Roles and Access
Donor: Can post available food details.

NGO: Can view donations and request pickup.

Admin: Manages users, NGOs, donation stats, and system settings.


### 1. Clone the Repository
```bash
git clone https://github.com/PrathameshBansode/Surplus-Food-Redistribution-System.git
