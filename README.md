# Smart Procurement Vendor Management System

**⚠️ CONFIDENTIAL - PRIVATE REPOSITORY**

This is a private enterprise application for internal use only.

---

## 📋 Overview

Smart Procurement Vendor Management System is an **enterprise-level full-stack application** designed to manage procurement operations and vendor relationships efficiently. Built with modern technologies and best practices.

---

## 🏗️ Architecture

### Full-Stack Application Structure

```
Smart-Procurement-Vendor-Management-System/
├── Frontend (React + Vite)
└── Backend (Spring Boot 4 + MySQL)
```

---

## 🛠️ Tech Stack

### **Frontend**
- **Framework:** React 19.2.0
- **Build Tool:** Vite 8.0.0-beta.13
- **Routing:** React Router DOM 7.13.0
- **HTTP Client:** Axios 1.13.5
- **Code Quality:** ESLint 9.39.1
- **Compiler:** React Compiler (enabled)

### **Backend**
- **Framework:** Spring Boot 4.0.2 (Java 21)
- **Database:** MySQL with Spring Data JPA
- **Security:** Spring Security
- **API:** Spring Web MVC (RESTful)
- **Build Tool:** Maven
- **ORM:** Hibernate JPA
- **Code Generation:** Lombok

### **Database**
- MySQL (primary database)

---

## ✨ Key Features

✅ **Procurement Management** - Handle procurement operations and workflows  
✅ **Vendor Management** - Manage vendor relationships and information  
✅ **Secure Authentication** - Spring Security-powered authentication & authorization  
✅ **RESTful APIs** - Clean, well-structured REST endpoints  
✅ **Responsive UI** - Modern React-based user interface  
✅ **Data Persistence** - Robust MySQL database integration  
✅ **Real-time Updates** - Axios-based API communication  

---

## 📦 Project Structure

```
Smart-Procurement-Vendor-Management-System/
│
├── Smart-Procurement-Vendor-Management-System-Backend-master/
│   ├── src/                          # Java source code
│   ├── pom.xml                       # Maven configuration
│   ├── mvnw / mvnw.cmd               # Maven wrapper
│   └── .mvn/                         # Maven settings
│
└── Smart-Procurement-Vendor-Management-System-Frontend-main/
    ├── src/                          # React components & logic
    ├── public/                       # Static assets
    ├── index.html                    # Application entry point
    ├── package.json                  # NPM dependencies
    ├── vite.config.js                # Vite configuration
    ├── eslint.config.js              # ESLint configuration
    └── .gitignore                    # Git ignore rules
```

---

## 🚀 Getting Started

### Prerequisites
- **Java 21+** (for backend)
- **Node.js 16+** (for frontend)
- **Maven 3.6+** (for backend build)
- **MySQL 8.0+** (for database)

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd Smart-Procurement-Vendor-Management-System-Backend-master
   ```

2. Build the project:
   ```bash
   mvn clean install
   ```

3. Run the application:
   ```bash
   mvn spring-boot:run
   ```

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd Smart-Procurement-Vendor-Management-System-Frontend-main
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start development server:
   ```bash
   npm run dev
   ```

4. Build for production:
   ```bash
   npm run build
   ```

---

## 🔐 Access & Support

This repository is restricted to **authorized team members only**.

For access requests or support:
- Contact your team lead
- Reach out to the development team

---

## 📄 License

**Proprietary - All rights reserved**

This project and all its contents are proprietary and confidential. Unauthorized copying, modification, or distribution is strictly prohibited.