# Task Management Application - Java Servlet Version

This is a Task Management Application built using Java Servlets for the backend, HTML/CSS/JavaScript for the frontend, and MySQL for data storage.

## Features
- User registration and login with session management
- Add, update, delete tasks with user-specific task lists
- MySQL database for storing users and tasks

## Prerequisites
- Java Development Kit (JDK) 8 or higher
- Apache Tomcat 9 or higher (or any Java Servlet container)
- MySQL Server
- Maven (optional, if using Maven for build)

## Setup Instructions

### 1. Clone or Download the Project
Download the project files to your local system.

### 2. Setup MySQL Database
- Create a new database named `task_management`.
- Run the provided SQL script `database.sql` to create the necessary tables.

Example:
```sql
CREATE DATABASE task_management;
USE task_management;

-- Run the SQL script provided in database.sql
```

### 3. Configure Database Connection
- Update the database connection settings in `src/main/resources/db.properties` or in the servlet code as needed (URL, username, password).

### 4. Build and Deploy the Application
- If using Maven, run:
```bash
mvn clean package
```
- Deploy the generated WAR file to your Tomcat server's `webapps` directory.
- Alternatively, copy the project folder to Tomcat's `webapps` directory if not using WAR.

### 5. Start Tomcat Server
- Start your Tomcat server.
- Access the application at: `http://localhost:8080/task-management/`

### 6. Using the Application
- Register a new user.
- Login with your credentials.
- Add, update, and delete your tasks.

## Project Structure
- `src/` - Java Servlet source code
- `web/` - HTML, JSP, CSS, JavaScript files
- `database.sql` - SQL script to create database tables

## Notes
- Ensure MySQL server is running before starting the application.
- Adjust database credentials as per your local setup.
- For any issues, check Tomcat logs for errors.

## Contact
For any questions or support, please contact the developer.
