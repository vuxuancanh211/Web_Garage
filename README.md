# 🚗 Garage Management System
A web-based system for managing vehicle maintenance and repair services at small-to-medium garages.

# 📌 Overview
Garage Management System is a web-based application designed to help small-to-medium garages efficiently manage their maintenance and repair operations.

The system provides a centralized platform for handling customer information, car service records, repair orders, and service scheduling. By replacing manual and paper-based processes, the application helps reduce operational errors, improve workflow efficiency, and enhance overall service quality.

With a clean and intuitive interface, garage staff can easily track service progress, manage repair histories, and maintain accurate records of all maintenance activities. The system supports role-based access control to ensure secure access to sensitive data and core functionalities.

This project is built using modern web technologies and follows a modular architecture, making it scalable, maintainable, and suitable for real-world garage environments.

# ✨ Features
For Customers
  - Register, log in, and manage personal profile
  - Book appointments online
  - View repair history with full cost breakdown
  - Submit feedback and complaints; receive management responses
  - Get maintenance suggestions and periodic reminders

For Employees
  - Create and manage appointments
  - Update repair and maintenance status
  - View assigned work orders and customer information

For Admin
  - Full management of customers, vehicles, employees, and branches
  - Manage repair orders, spare parts inventory, and services catalog
  - Handle customer complaints and feedback
  - View revenue reports and statistics
  - AI chatbot with RAG (Retrieval-Augmented Generation) for service queries 

#  🛠️ Tech Stack
  - Java + Spring Boot 3
  - Spring Security + JWT
  - Spring Data JPA + Hibernate
  - PostgreSQL
  - pgvector
  - React + Vite
  - Tailwind CSS
  - Gemini AI
  - Cloudinary
  - Docker

# 🚀 Getting Started
### 1. Prerequisites
  - Java 17+
  - Maven
  - Docker
  - PostgreSQL

### 2. Clone Repository
```bash
git clone https://github.com/vuxuancanh211/Web_Garage.git
cd Web_garage
```

### 3. Configure Environment Variables
Create .env file
  - DB_USERNAME=your_db_username
  - DB_PASSWORD=your_db_password

  - JWT_SECRET=your_jwt_secret
  - JWT_EXPIRATION=86400000

  - GEMINI_API_KEY=your_gemini_api_key

  - CLOUDINARY_NAME=your_cloud_name
  - CLOUDINARY_KEY=your_cloud_key
  - CLOUDINARY_SECRET=your_cloud_secret

  - MAIL_USERNAME=your_email@gmail.com
  - MAIL_PASSWORD=your_app_password

### 4. Run Application
Database
```bash
cd docker
docker-compose up -d
```

Application
```bash
Find application.properties
Modify init sql mode from never to always
```
```bash
cd ..
mvn clean package
java "-Duser.timezone=Asia/Ho_Chi_Minh" -jar target\garage-0.0.1-SNAPSHOT.jar
```

# Admin Account
- admin@gara.com
- 123456
