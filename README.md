# Opti-Reserve
## Smart Facility & Resource Management System


Opti-Reserve is a full-stack facility and resource management system designed to simplify the booking, scheduling, and management of university resources including laboratories, auditoriums, meeting rooms, seminar halls, and equipment.

The system provides centralized resource management, reservation handling, user authentication, role-based access control, maintenance reporting, and analytics.

---

# 🚀 Features

## User Management
- User registration and authentication
- JWT-based authentication
- Role-based authorization
- Admin and user access control

## Resource Management
- Create and manage resources
- Categorize facilities
- Search and filter available resources
- Resource availability tracking

## Reservation System
- Create resource bookings
- View reservation schedules
- Prevent booking conflicts
- Manage reservation status

## Check-In / Check-Out Management
- Track resource usage
- Mark no-show reservations
- Maintain usage history

## Maintenance Reporting
- Report damaged resources
- Track maintenance requests
- Update repair status

## Open Session Publishing
- Publish available resources
- Allow users to discover open sessions

## Reporting & Analytics
- Reservation statistics
- Resource utilization reports
- Usage monitoring

---

# 🛠 Tech Stack

## Frontend

- React.js
- Vite
- Tailwind CSS
- JavaScript
- HTML5
- CSS3

## Backend

- ASP.NET Core Web API
- C#
- Entity Framework Core
- ASP.NET Identity
- JWT Authentication

## Database

- SQLite
- Entity Framework Core ORM
- LINQ

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
REST API
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

Opti-Reserve uses SQLite as the database with Entity Framework Core for ORM.

Main entities:

## Users

Stores system users and authentication information.

Fields:

- UserId
- Name
- Email
- PasswordHash
- Role


## Resources

Stores available university facilities.

Fields:

- ResourceId
- ResourceName
- Category
- Location
- AvailabilityStatus


## Reservations

Stores booking information.

Fields:

- ReservationId
- UserId
- ResourceId
- StartTime
- EndTime
- Status


## Maintenance Reports

Stores resource maintenance issues.

Fields:

- ReportId
- ResourceId
- Description
- Status
- CreatedDate


---

# ⚙️ Installation Guide

## Prerequisites

Install:

- .NET 8 SDK
- Node.js
- Git

---

# Backend Setup

Clone repository:

```bash
git clone https://github.com/yourusername/Opti-Reserve.git

Navigate:

cd Backend

Install dependencies:

dotnet restore

Apply database migration:

dotnet ef database update

Run backend:

dotnet run

Backend runs on:

http://localhost:5121
Frontend Setup

Navigate:

cd Frontend

Install packages:

npm install

Run application:

npm run dev

Frontend runs on:

http://localhost:5173
