# Doctor Appointment Web App

A full-featured Doctor Appointment Web Application built with **PHP, MySQL, and WebRTC**, designed to streamline patient-doctor interactions. This project includes authentication, appointment booking, real-time video consultations, an SOS alert system, and admin management.  

---

## Table of Contents

- [Features](#features)  
- [Tech Stack](#tech-stack)  
- [Installation](#installation)  
- [Configuration](#configuration)  
- [Database Setup](#database-setup)  
- [Project Structure](#project-structure)  
- [Usage](#usage)  
- [Future Enhancements](#future-enhancements)  
- [Contributing](#contributing)  
- [License](#license)  

---

## Features

### Authentication
- Complete **Doctor and Patient authentication**
  - Registration, login, logout
  - Email verification
  - Password reset via email
- Secure password storage using `password_hash()` and `password_verify()`
- Session management and role-based access
- Failed login throttling

### Doctor Panel
- Dashboard with appointment statistics
- Profile management with photo uploads
- Availability scheduling
- Appointment management (list, update status)
- Video consultation management (WebRTC)

### Patient Panel
- Dashboard with upcoming/past appointments
- Profile management
- Searchable doctor directory with filters:
  - Specialization, experience, rating, hospital, availability
- Appointment booking with dynamic time slot availability
- My Appointments section
- Video consultation with doctors (WebRTC)

### SOS Emergency System
- Trigger SOS alerts from patient or doctor panel
- Admin panel integration to monitor alerts
- Responder logic with notifications via SMS, email, and push
- PWA-enabled emergency trigger with experimental power-button simulation

### Admin Panel
- Manage Doctors, Patients, Appointments
- Approve or reject doctors
- View SOS alerts and logs

---

## Tech Stack

- **Backend:** PHP 8+, PDO (MySQL prepared statements)  
- **Frontend:** HTML, CSS, JavaScript  
- **Database:** MySQL  
- **Real-time:** WebRTC (video & chat)  
- **Notifications:** Twilio (SMS), SendGrid (Email), Firebase Cloud Messaging (Push)  
- **Maps & Geolocation:** Google Maps API  
- **File Storage:** AWS S3 / Cloudinary / Local `/uploads`  
- **Monitoring:** Sentry, LogRocket  

---

## Installation

1. Clone the repository:  
```bash
git clone https://github.com/yourusername/doctor-appointment-app.git
cd doctor-appointment-app
