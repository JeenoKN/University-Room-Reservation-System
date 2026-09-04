# University Room Reservation & Management System

A full-stack university room reservation system designed for students, lecturers, and staff.

The application supports role-based room booking, approval workflows, room management, booking history, and automatic handling of expired booking requests.

## Features

### Student
- Register and log in
- Browse available rooms
- Submit room reservation requests
- Cancel reservations
- View booking status and booking history

### Lecturer
- Review reservation requests
- Approve or reject bookings
- View approval history

### Staff
- Add and manage rooms
- Update room availability
- View reservation activity and booking history

### System
- Session-based authentication
- Password hashing
- Role-based access control
- RESTful API architecture
- MySQL database integration
- Automatic handling of expired booking requests with scheduled jobs

## Tech Stack

### Frontend
- Flutter
- Dart

### Backend
- Node.js
- Express.js

### Database
- MySQL

### Authentication & Backend Utilities
- Express Session
- bcrypt
- Node Cron
- CORS

## System Architecture

```text
Flutter Application
        |
        | REST API
        v
Node.js + Express
        |
        v
      MySQL
```

## User Roles

Protected backend functionality is separated by role:

```text
Student  -> browse rooms, create bookings, cancel bookings, view history
Lecturer -> review requests, approve/reject bookings, view approval history
Staff    -> manage rooms, availability, and booking activity
```

## Getting Started

### Requirements

- Flutter SDK
- Node.js
- MySQL
- Git

### 1. Clone the repository

```bash
git clone https://github.com/JeenoKN/University-Room-Reservation-System.git
cd University-Room-Reservation-System
```

### 2. Install Flutter dependencies

```bash
flutter pub get
```

### 3. Install backend dependencies

```bash
cd backend
npm install
```

### 4. Configure environment variables

Copy `backend/.env.example` to `backend/.env` and update the values for your local MySQL setup.

```env
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=room_booking
DB_PORT=3306
```

Do not commit your real `.env` file to GitHub.

### 5. Start the backend

```bash
node server.js
```

### 6. Run the Flutter application

From the project root:

```bash
flutter run
```

## Project Type

Course Project  
Bachelor of Engineering in Computer Engineering

## Author

**Theeramonrapat Vichaisri**  
Computer Engineering Student
