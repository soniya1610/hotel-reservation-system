# 🏨 Hotel Reservation System

A console-based **Java backend project** built using **JDBC** and **MySQL** for managing hotel room reservations.  
This project allows users to reserve rooms, view reservations, update booking details, and delete reservations through a menu-driven interface.

---

## 📌 Project Overview

The Hotel Reservation System is designed to simplify reservation management in hotels.  
It provides a command-line interface (CLI) where users can perform CRUD operations on reservation data stored in a MySQL database.

This project helped me strengthen my understanding of:

- Java programming
- JDBC connectivity
- SQL queries
- CRUD operations
- Exception handling

---

## ✨ Features

✅ Reserve a room  
✅ View all reservations  
✅ Get room number using reservation ID  
✅ Update reservation details  
✅ Delete reservation  
✅ Menu-driven CLI interface  
✅ Database integration using JDBC  

---

## 🛠 Tech Stack

- **Java**
- **JDBC**
- **MySQL**
- **SQL**
- **IntelliJ IDEA**

---

## 📂 Project Structure

```bash
hotel-reservation-system/
│
├── Hotel Reservation System/
│   └── HotelReservationSystem.java
│
├── .gitignore
└── README.md
```

---

## ⚙️ Setup Instructions

### 1. Clone Repository
```bash
git clone https://github.com/soniya1610/hotel-reservation-system.git
```

### 2. Open in IntelliJ IDEA
Import the project into IntelliJ.

### 3. Setup MySQL Database
Create database:

```sql
CREATE DATABASE hotel_db;
```

### 4. Create Table

```sql
CREATE TABLE reservations (
    res_id INT PRIMARY KEY AUTO_INCREMENT,
    guest_name VARCHAR(100) NOT NULL,
    room_number INT NOT NULL,
    contact_number VARCHAR(10) NOT NULL,
    reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

### 5. Update Database Credentials
Update these values in Java code:

```java
private static final String url = "jdbc:mysql://localhost:3306/hotel_db";
private static final String username = "root";
private static final String password = "<your_password>";
```

### 6. Run the Project
Run `HotelReservationSystem.java`

---

## 🗄 Database Schema

| Column Name | Data Type | Description |
|------------|-----------|-------------|
| res_id | INT | Reservation ID (Primary Key) |
| guest_name | VARCHAR(100) | Guest Name |
| room_number | INT | Room Number |
| contact_number | VARCHAR(10) | Contact Number |
| reservation_date | TIMESTAMP | Booking Timestamp |

---

## 📷 Sample Menu

```text
Hotel Management System
1. Reserve a room
2. View Reservations
3. Get Room Number
4. Update Reservations
5. Delete Reservations
0. Exit
```


## 👩‍💻 Author

**Soniya Meena**  
B.Tech CSE Student | Java Backend Learner  
GitHub: https://github.com/soniya1610
