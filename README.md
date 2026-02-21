# Library Management System

## Description
The Library Management System is a web-based application designed to streamline the processes involved in managing a library. It includes functionalities designed to enhance user experience and improve the overall efficiency of library operations.

## Features
- **User Registration**: Allow users to create accounts to access library services.
- **Book Catalog Management**: Manage a comprehensive catalog of books available in the library.
- **Borrowing and Returning Books**: Facilitate the process of borrowing and returning books in an organized manner.
- **Search Functionality**: Enable users to search for books based on various criteria such as title, author, and genre.
- **Reporting Tools**: Generate reports concerning library usage and statistics to aid in management decisions.

## Project Structure
```
library-management-system/
├── frontend/                 # React TypeScript Frontend
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── styles/
│   │   ├── App.tsx
│   │   └── main.tsx
│   ├── package.json
│   └── vite.config.ts
├── backend/                  # Spring Boot Backend
│   ├── src/main/java/com/library/
│   │   ├── entity/
│   │   ├── repository/
│   │   ├── service/
│   │   ├── controller/
│   │   ├── dto/
│   │   ├── exception/
│   │   └── LibraryManagementSystemApplication.java
│   ├── src/main/resources/
│   │   └── application.properties
│   └── pom.xml
└── SETUP.md
```

## Technologies Used
- **Frontend**: React 18, TypeScript, Vite, Axios
- **Backend**: Spring Boot 3.0, Java 17, Spring Data JPA
- **Database**: MySQL 8.0
- **Build Tools**: Maven, npm

## API Endpoints
- `GET /api/books` - Get all books
- `GET /api/books/{id}` - Get book by ID
- `POST /api/books` - Create a new book
- `PUT /api/books/{id}` - Update a book
- `DELETE /api/books/{id}` - Delete a book

## Getting Started
See SETUP.md for detailed installation and configuration instructions.

## License
MIT License