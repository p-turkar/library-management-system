# Library Management System - Setup Guide

## Prerequisites
- Node.js (v16+)
- Java JDK 17+
- MySQL 8.0+
- Maven 3.6+
- Git

## Frontend Setup (React)

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

The frontend will be available at `http://localhost:5173`

## Backend Setup (Spring Boot)

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Create MySQL Database:
   ```sql
   CREATE DATABASE library_db;
   ```

3. Build the project:
   ```bash
   mvn clean install
   ```

4. Run the application:
   ```bash
   mvn spring-boot:run
   ```

The backend API will be available at `http://localhost:8080/api`

## API Endpoints

### Books
- `GET /api/books` - Get all books
- `GET /api/books/{id}` - Get book by ID
- `POST /api/books` - Create a new book
- `PUT /api/books/{id}` - Update a book
- `DELETE /api/books/{id}` - Delete a book

## Database Configuration

Update `backend/src/main/resources/application.properties`:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/library_db
spring.datasource.username=root
spring.datasource.password=root
```

## Project Structure
```
library-management-system/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── styles/
│   │   ├── App.tsx
│   │   └── main.tsx
│   ├── package.json
│   └── vite.config.ts
├── backend/
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
└── README.md
```

## Features

✅ CRUD Operations for Books  
✅ RESTful API  
✅ Responsive UI  
✅ Error Handling  
✅ Database Persistence  
✅ CORS Support

## Troubleshooting

**Backend Connection Error:**
- Ensure MySQL is running
- Check database credentials in `application.properties`

**Frontend Connection Error:**
- Verify backend is running on port 8080
- Check CORS configuration

**Port Already in Use:**
- Change port in configuration and restart the server

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.