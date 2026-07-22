# Opti-Reserve
## Smart Facility & Resource Management System

## 📌 Overview

**Opti-Reserve** is a full-stack Smart Facility & Resource Management System designed to simplify the booking, scheduling, and management of university resources including laboratories, auditoriums, seminar halls, meeting rooms, and equipment.

The system provides a centralized platform for resource management, reservation handling, user authentication, role-based access control, maintenance reporting, check-in/check-out tracking, and resource utilization analytics.

This project is developed as a **Final Year Project (FYP)** for the **BS Software Engineering program at SZABIST Karachi**.

---

# 🎯 Project Objectives

- Replace manual facility booking processes with a digital management system.
- Reduce resource scheduling conflicts and double bookings.
- Provide administrators with complete control over university resources.
- Improve transparency through reservation tracking.
- Enable efficient maintenance reporting and monitoring.
- Provide analytics for better resource utilization decisions.

---

# 🚀 Features

## 👤 User Management

- User registration and authentication
- JWT-based authentication
- Secure user login system
- Role-based authorization
- Admin and user access control

---

## 🏢 Resource Management

- Create and manage university resources
- Manage resource categories
- Search and filter available resources
- Track resource availability status
- Maintain resource information

---

## 📅 Reservation Management

- Create resource bookings
- View reservation schedules
- Prevent booking conflicts
- Manage reservation status
- Maintain booking history

---

## ✅ Check-In / Check-Out Management

- Track resource usage
- Record user check-ins and check-outs
- Mark no-show reservations
- Maintain resource usage history

---

## 🔧 Maintenance Reporting

- Report damaged resources
- Submit maintenance requests
- Track repair progress
- Update maintenance status

---

## 📢 Open Session Publishing

- Publish available resource sessions
- Allow users to discover available resources
- Improve resource utilization

---

## 📊 Reporting & Analytics

- Reservation statistics
- Resource utilization reports
- Usage monitoring
- Administrative insights

---

# 🛠 Tech Stack

## Frontend

- React.js
- Vite
- Tailwind CSS
- JavaScript
- HTML5
- CSS3

---

## Backend

- ASP.NET Core Web API
- C#
- Entity Framework Core
- ASP.NET Identity
- JWT Authentication
- RESTful APIs

---

## Database

- SQLite
- Entity Framework Core ORM
- LINQ

---

## Development Tools

- Visual Studio Code
- Visual Studio
- Git & GitHub
- Swagger UI
- Postman

---

# 🏗 System Architecture

          React Frontend
                |
                |
          RESTful API
                |
                |
      ASP.NET Core Web API
                |
                |
      Entity Framework Core
                |
                |
         SQLite Database

---

# 🗄 Database Design

Opti-Reserve uses **SQLite** as the database with **Entity Framework Core ORM** for database management.

## Main Entities

---

## Users

Stores authentication and user information.

Fields:


UserId
Name
Email
PasswordHash
Role


---

## Resources

Stores university facilities and available resources.

Fields:


ResourceId
ResourceName
Category
Location
AvailabilityStatus


---

## Reservations

Stores resource booking information.

Fields:


ReservationId
UserId
ResourceId
StartTime
EndTime
Status


---

## Maintenance Reports

Stores resource maintenance issues.

Fields:


ReportId
ResourceId
Description
Status
CreatedDate


---

# 📂 Project Structure


Opti-Reserve

│
├── Backend
│ ├── Controllers
│ ├── Models
│ ├── DTOs
│ ├── Services
│ ├── Data
│ ├── Migrations
│ └── Program.cs
│
├── Frontend
│ ├── src
│ ├── components
│ ├── pages
│ └── services
│
└── README.md


---

# ⚙️ Installation Guide

## Prerequisites

Install the following:

- .NET 8 SDK
- Node.js
- Git

---

# Backend Setup

### Clone Repository

```bash
git clone https://github.com/omrohra220/Opti-Reserve.git
Navigate to Backend
cd Backend
Restore Dependencies
dotnet restore
Apply Database Migration
dotnet ef database update
Run Backend Server
dotnet run

Backend will run on:

http://localhost:5121

Swagger API Documentation:

http://localhost:5121/swagger
Frontend Setup

Navigate to frontend folder:

cd Frontend

Install dependencies:

npm install

Start development server:

npm run dev

Frontend will run on:

http://localhost:5173
🔐 Security Implementation

Security features implemented:

JWT Authentication
Password hashing
Role-based authorization
Protected API endpoints
Secure user access management
🔮 Future Enhancements

Possible future improvements:

Email notification system
Calendar integration
Cloud deployment
Mobile application
Advanced analytics dashboard
AI-based resource recommendation system
👨‍💻 Developer

Om Rohra

BS Software Engineering
SZABIST Karachi

GitHub:

https://github.com/omrohra220

📄 License

This project was developed as a Final Year Project.

