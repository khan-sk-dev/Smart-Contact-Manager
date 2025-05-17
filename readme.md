# 📇 Smart Contact Manager

<div align="center">

![Smart Contact Manager Banner](https://img.shields.io/badge/Smart-Contact%20Manager-1DA1F2?style=for-the-badge&logo=address-book&logoColor=white)

[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=spring&logoColor=white)](https://spring.io/projects/spring-boot)
[![Thymeleaf](https://img.shields.io/badge/Thymeleaf-005F0F?style=for-the-badge&logo=thymeleaf&logoColor=white)](https://www.thymeleaf.org/)
[![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)

</div>

A powerful Spring Boot-based Contact Management System (CMS) designed to provide a user-friendly interface for managing personal contacts with advanced features like search, pagination, and profile management.

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Features](#-features)
- [Technologies Used](#-technologies-used)
- [REST API Endpoints](#-rest-api-endpoints)
- [Project Structure](#-project-structure) 
- [Getting Started](#-getting-started)
- [Screenshots](#-screenshots)
- [License](#-license)
- [Author](#-author)

---

## 🔍 Project Overview

Smart Contact Manager is a comprehensive application designed to provide a user-friendly interface for managing personal contacts. It enables users to register, log in, and maintain a list of contacts, which can include details like name, email, phone number, and profile picture. The system offers a seamless experience with intuitive search functionality, pagination for large contact lists, and secure user authentication.

---

## 🌟 Features

- **User Authentication**
  - Secure user authentication using Spring Security
  - User registration with email verification
  - Password management with encryption

- **User Profile Management**
  - Create and update user profiles
  - Personalized dashboard for each user
  - User-specific settings and preferences

- **Contact Management**
  - Add new contacts with comprehensive details
  - View contacts with efficient pagination
  - Advanced search by name, email, or phone number
  - Edit and delete contacts with ease
  - Contact categorization and organization

- **Media Management**
  - Upload profile pictures for contacts
  - Cloudinary integration for secure image storage
  - Image optimization and thumbnail generation

- **User Experience**
  - Responsive design using Tailwind CSS
  - Custom flash messages for user feedback
  - Intuitive navigation and user interface
  - Cross-device compatibility

- **API Access**
  - RESTful API endpoints for programmatic access
  - Secure API authentication
  - JSON data format for easy integration

---

## 💻 Technologies Used

| Category | Technologies |
|----------|-------------|
| **Backend** | Spring Boot, Spring Security, Spring Data JPA (Hibernate) |
| **Frontend** | Thymeleaf, HTML5, Tailwind CSS, JavaScript |
| **Database** | MySQL |
| **Cloud Services** | Cloudinary (Image Upload) |
| **Validation** | JSR-303 (via Hibernate Validator) |
| **Logging** | SLF4J with Logback |
| **Containerization** | Docker, Docker Compose |
| **Build Tool** | Maven |
| **Version Control** | Git, GitHub |

---

## 🔄 REST API Endpoints

### User Endpoints

| Method | URL | Description |
|--------|-----|-------------|
| GET | `/user/dashboard` | User dashboard page |
| GET | `/user/profile` | User profile page |

### Contact Management Endpoints

| Method | URL | Description |
|--------|-----|-------------|
| GET | `/user/contacts/add` | View add contact page |
| POST | `/user/contacts/add` | Add a new contact |
| GET | `/user/contacts` | View all contacts with pagination |
| GET | `/user/contacts/search` | Search for contacts |
| DELETE | `/user/contacts/delete/{contactId}` | Delete a contact by ID |
| GET | `/user/contacts/view/{contactId}` | View contact update page by ID |
| POST | `/user/contacts/update/{contactId}` | Update an existing contact by ID |

### Public Pages

| Method | URL | Description |
|--------|-----|-------------|
| GET | `/home` | Home page |
| GET | `/about` | About page |
| GET | `/services` | Services page |
| GET | `/contact` | Contact page |

### Authentication Endpoints

| Method | URL | Description |
|--------|-----|-------------|
| GET | `/login` | Login page |
| GET | `/register` | Registration page |
| POST | `/do-register` | Process registration |

### API Endpoints

| Method | URL | Description |
|--------|-----|-------------|
| GET | `/api/contacts/{contactId}` | Retrieve contact details by ID |

---

## 📂 Project Structure

```
src
├── main
│   ├── java
│   │   └── com
│   │       └── scm
│   │           ├── controllers   // Controllers for handling user requests
│   │           ├── entities      // JPA entities representing data models
│   │           ├── forms         // Form objects for request validation
│   │           ├── helpers       // Utility classes for common functionalities
│   │           ├── services      // Service layer for business logic
│   └── resources
│       ├── templates             // Thymeleaf templates for frontend pages
│       ├── application.properties // Application configurations
└── test
    └── java
        └── com
            └── scm
                └── tests         // Unit tests for the application
```

---

## 🚀 Getting Started

### Prerequisites

- JDK 11 or higher
- Maven 3.6+
- MySQL 8.0+
- Docker (optional, for containerized deployment)

### Installation

#### Standard Setup

```bash
# Clone the repository
git clone https://github.com/khan-sk-dev/Smart-Contact-Manager.git
cd Smart-Contact-Manager

# Build the project
mvn clean install

# Run the application
mvn spring-boot:run
```

#### Docker Setup

```bash
# Clone the repository
git clone https://github.com/khan-sk-dev/Smart-Contact-Manager.git
cd Smart-Contact-Manager

# Build and run with Docker Compose
docker-compose up --build
```

### Configuration

Update `application.properties` with your database credentials:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/contactmanager
spring.datasource.username=your_username
spring.datasource.password=your_password
```

For Cloudinary configuration:

```properties
cloudinary.cloud-name=your_cloud_name
cloudinary.api-key=your_api_key
cloudinary.api-secret=your_api_secret
```

---

## 📸 Screenshots

<div align="center">
  <i>Screenshots coming soon!</i>
</div>

---


## 👨‍💻 Author

**صہیب خان** – [GitHub](https://github.com/khan-sk-dev)

---

<div align="center">
  
  ⭐ **Star this repo if you find it useful!** ⭐
  
  <a href="https://github.com/khan-sk-dev/Smart-Contact-Manager/stargazers">
    <img src="https://img.shields.io/github/stars/khan-sk-dev/Smart-Contact-Manager?style=social" alt="Stars"/>
  </a>
  
</div>
