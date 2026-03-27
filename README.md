# 🚀 Smart Procurement Vendor Management System

> A cutting-edge full-stack enterprise solution for intelligent procurement and vendor lifecycle management

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Java](https://img.shields.io/badge/Java-21-orange.svg)
![React](https://img.shields.io/badge/React-19-cyan.svg)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-4.0.2-brightgreen.svg)

## 📋 Table of Contents
- [Overview](#overview)
- [Architecture](#architecture)
- [Tech Stack](#tech-stack)
- [Features](#features)
- [Quick Start](#quick-start)
- [Project Structure](#project-structure)
- [Backend Setup](#backend-setup)
- [Frontend Setup](#frontend-setup)
- [Database Configuration](#database-configuration)
- [API Documentation](#api-documentation)
- [Contributing](#contributing)
- [License](#license)

---

## 🎯 Overview

The **Smart Procurement Vendor Management System** is an enterprise-grade platform designed to revolutionize how organizations manage their procurement processes and vendor relationships. Built with modern technologies, it provides intelligent vendor evaluation, automated procurement workflows, and comprehensive analytics.

### Key Capabilities
- 🎪 **Multi-vendor Management**: Handle complex vendor ecosystems with ease
- 📊 **Smart Analytics**: Real-time insights into procurement metrics and vendor performance
- 🔐 **Enterprise Security**: Role-based access control and data protection
- ⚡ **High Performance**: Optimized for scalability and responsiveness
- 📱 **Responsive Design**: Works seamlessly across all devices

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                     Frontend (React 19)                      │
│              Smart UI with Responsive Design                 │
└────────────────────────────┬────────────────────────────────┘
                             │
                    (Axios HTTP Client)
                             │
┌────────────────────────────▼────────────────────────────────┐
│            Backend API (Spring Boot 4.0.2)                   │
│          Java 21 | RESTful Services | Security               │
└────────────────────────────┬────────────────────────────────┘
                             │
┌────────────────────────────▼────────────────────────────────┐
│         Database Layer (MySQL with JPA/Hibernate)            │
│            Data Persistence & Query Optimization             │
└─────────────────────────────────────────────────────────────┘
```

---

## 🛠️ Tech Stack

### Backend
```
Framework:     Spring Boot 4.0.2
Language:      Java 21
Build Tool:    Maven
ORM:           JPA (Java Persistence API)
Database:      MySQL
Security:      Spring Security
Code Gen:      Project Lombok
```

### Frontend
```
Framework:     React 19.2.0
Build Tool:    Vite 8.0.0-beta
Language:      Modern JavaScript (ES Modules)
HTTP Client:   Axios 1.13.5
Routing:       React Router DOM 7.13.0
Linting:       ESLint 9.39.1
Type Checking: TypeScript Support
```

### Key Dependencies

**Backend Dependencies:**
- `spring-boot-starter-data-jpa` - ORM and database access
- `spring-boot-starter-security` - Authentication & authorization
- `spring-boot-starter-webmvc` - REST API development
- `mysql-connector-j` - MySQL database driver
- `lombok` - Reduces boilerplate code

**Frontend Dependencies:**
- `react` & `react-dom` - UI library
- `react-router-dom` - Client-side routing
- `axios` - HTTP client for API calls
- `@vitejs/plugin-react` - React support in Vite
- `eslint` - Code quality & linting

---

## ✨ Features

### Core Capabilities
✅ **Vendor Management**
- Complete vendor lifecycle management
- Performance tracking and analytics
- Automated vendor evaluation metrics
- Multi-tier vendor classification

✅ **Procurement Operations**
- Purchase order generation and tracking
- Automated approval workflows
- Real-time status monitoring
- Historical audit trails

✅ **Security & Access Control**
- Role-based access control (RBAC)
- Spring Security integration
- Secure authentication mechanisms
- Data encryption and protection

✅ **Analytics & Reporting**
- Vendor performance dashboards
- Procurement insights
- Cost analysis tools
- Custom report generation

✅ **User Experience**
- Intuitive modern interface
- Mobile-responsive design
- Real-time notifications
- Dark/Light theme support

---

## 🚀 Quick Start

### Prerequisites
- ☕ Java 21 or higher
- 📦 Node.js 16+ & npm
- 🗄️ MySQL 5.7+
- 🔧 Maven 3.8+
- 🎨 Git

### Installation Steps

#### 1️⃣ Clone the Repository
```bash
git clone https://github.com/KAMALIV-06/Smart-Procurement-Vendor-Management-System.git
cd Smart-Procurement-Vendor-Management-System
```

#### 2️⃣ Backend Setup
```bash
cd Smart-Procurement-Vendor-Management-System-Backend-master/SmartProcurementVendorManagementSystemProject
mvn clean install
mvn spring-boot:run
```
Backend runs on: `http://localhost:8080`

#### 3️⃣ Frontend Setup
```bash
cd Smart-Procurement-Vendor-Management-System-Frontend-main
npm install
npm run dev
```
Frontend runs on: `http://localhost:5173`

#### 4️⃣ Access the Application
Open your browser and navigate to: `http://localhost:5173`

---

## 📁 Project Structure

```
Smart-Procurement-Vendor-Management-System/
│
├── Smart-Procurement-Vendor-Management-System-Backend-master/
│   ├── SmartProcurementVendorManagementSystemProject/
│   │   ├── src/main/java/
│   │   │   └── com/smartprocurementvendormanagementsystem/
│   │   │       ├── controller/        # REST endpoints
│   │   │       ├── service/           # Business logic
│   │   │       ├── repository/        # Data access layer
│   │   │       ├── model/             # Entity classes
│   │   │       ├── security/          # Security configs
│   │   │       └── exception/         # Custom exceptions
│   │   ├── src/main/resources/
│   │   │   ├── application.properties # Configuration
│   │   │   └── db/                    # Database scripts
│   │   └── pom.xml
│   │
│   └── pom.xml (Parent POM)
│
├── Smart-Procurement-Vendor-Management-System-Frontend-main/
│   ├── src/
│   │   ├── components/        # React components
│   │   ├── pages/             # Page components
│   │   ├── services/          # API services
│   │   ├── hooks/             # Custom hooks
│   │   ├── utils/             # Utility functions
│   │   ├── styles/            # CSS & styling
│   │   ├── App.jsx            # Root component
│   │   └── main.jsx           # Entry point
│   ├── package.json
│   ├── vite.config.js
│   └── eslint.config.js
│
└── README.md (You are here!)
```

---

## ⚙️ Backend Setup

### Database Configuration
Edit `application.properties`:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/smart_procurement_db
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

### Build & Run
```bash
# Build the project
mvn clean build

# Run the application
mvn spring-boot:run

# Or run the JAR directly
java -jar target/SmartProcurementVendorManagementSystemProject-0.0.1-SNAPSHOT.jar
```

### Run Tests
```bash
mvn test
```

---

## 🎨 Frontend Setup

### Development Server
```bash
npm run dev
```

### Production Build
```bash
npm run build
npm run preview
```

### Code Quality
```bash
# Run ESLint
npm run lint

# Fix linting issues
npm run lint -- --fix
```

---

## 🗄️ Database Configuration

### MySQL Setup
```sql
-- Create database
CREATE DATABASE smart_procurement_db CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;

-- Use database
USE smart_procurement_db;

-- Tables are auto-generated by Hibernate (if using ddl-auto=update)
```

### Entity Models
Key entities managed by JPA:
- **Vendor** - Vendor information and details
- **ProcurementOrder** - Purchase orders
- **Approval** - Workflow approvals
- **Analytics** - Performance metrics
- **User** - User accounts and permissions

---

## 📡 API Documentation

### Base URL
```
http://localhost:8080/api
```

### Authentication
All endpoints (except login) require Bearer token:
```
Authorization: Bearer <jwt_token>
```

### Sample Endpoints

#### Vendors
```
GET    /api/vendors              # Get all vendors
POST   /api/vendors              # Create vendor
GET    /api/vendors/{id}         # Get vendor details
PUT    /api/vendors/{id}         # Update vendor
DELETE /api/vendors/{id}         # Delete vendor
```

#### Procurement Orders
```
GET    /api/orders               # List orders
POST   /api/orders               # Create order
GET    /api/orders/{id}          # Get order details
PUT    /api/orders/{id}          # Update order
DELETE /api/orders/{id}          # Cancel order
```

#### Analytics
```
GET    /api/analytics/dashboard  # Dashboard metrics
GET    /api/analytics/vendors    # Vendor performance
GET    /api/analytics/orders     # Order statistics
```

---

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. **Fork the Repository**
   ```bash
   git clone https://github.com/KAMALIV-06/Smart-Procurement-Vendor-Management-System.git
   ```

2. **Create Feature Branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```

3. **Commit Changes**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```

4. **Push to Branch**
   ```bash
   git push origin feature/AmazingFeature
   ```

5. **Open Pull Request**
   - Describe your changes clearly
   - Reference any related issues
   - Ensure all tests pass

### Development Guidelines
- Follow Java/JavaScript naming conventions
- Write meaningful commit messages
- Add tests for new features
- Keep code DRY and maintainable
- Update documentation as needed

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙋 Support & Questions

- 📧 **Email**: kamaliv.dev@example.com
- 🐛 **Issues**: [GitHub Issues](https://github.com/KAMALIV-06/Smart-Procurement-Vendor-Management-System/issues)
- 💬 **Discussions**: [GitHub Discussions](https://github.com/KAMALIV-06/Smart-Procurement-Vendor-Management-System/discussions)

---

## 🌟 Show Your Support

If this project helps you, please consider:
- ⭐ Starring the repository
- 🔗 Sharing with your network
- 🐛 Reporting issues
- 💡 Suggesting improvements

---

<div align="center">

**Built with ❤️ by [KAMALIV-06](https://github.com/KAMALIV-06)**

Made with ☕ Java, ⚛️ React, and 🚀 Spring Boot

</div>
