# Employee Management System

A Java-based Employee Management System developed as a technical assessment project. The application demonstrates employee registration, login, validation, and employee management using the Spring MVC framework and Hibernate.

## Features

- Employee registration
- Employee login
- Server-side form validation
- Display employee records
- Exclude the currently logged-in employee from the employee listing
- Database integration using Hibernate

## Technologies Used

| Technology | Purpose |
|---|---|
| Java 11 | Backend development |
| Spring MVC 5 | Web application framework |
| Spring ORM | ORM integration |
| Hibernate 5 | Database persistence |
| HibernateTemplate | Database operations |
| JSP | View layer |
| MySQL | Relational database |
| Maven | Dependency management and build |
| Apache Tomcat 9 | Application server |
| HTML / CSS | Frontend |

## Project Architecture

The application follows a layered architecture:

```text
JSP Views
   |
Controller Layer
   |
Service Layer
   |
DAO Layer
   |
HibernateTemplate
   |
MySQL Database
```

### Main Components

- **Controller:** Handles HTTP requests and manages application navigation.
- **Service:** Contains business logic.
- **DAO:** Handles database operations.
- **Entity:** Represents database entities.
- **JSP:** Provides the application's user interface.

## Project Structure

```text
OaklandTask/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/oakland/
│       │       ├── controller/
│       │       ├── service/
│       │       ├── dao/
│       │       └── entity/
│       └── webapp/
│           └── WEB-INF/
│               ├── spring-servlet.xml
│               └── *.jsp
├── pom.xml
└── README.md
```

## Prerequisites

Make sure the following software is installed:

- JDK 11
- Apache Maven
- MySQL Server
- Apache Tomcat 9

## Database Configuration

1. Create a MySQL database for the application.
2. Configure the database connection in `spring-servlet.xml`.
3. Update the database URL, username, and password according to your local MySQL configuration.
4. Ensure that the configured database and user are accessible.

**Important:** Do not commit personal database credentials or other sensitive configuration values to GitHub. Use environment variables or an external configuration file for local development.

## Build and Run

**1. Clone the repository**

```bash
git clone https://github.com/Sunilmaske12/Java-Technical-Assessment.git
```

**2. Navigate to the project directory**

```bash
cd Java-Technical-Assessment/OaklandTask
```

**3. Build the project**

```bash
mvn clean package
```

**4. Deploy to Apache Tomcat**

- Copy the generated WAR file from the `target` directory into Tomcat's `webapps` directory.
- Start the Tomcat server.
- Open the application in your browser using the appropriate context path.

## Learning Objectives

This project demonstrates practical implementation of:

- Java web application development
- Spring MVC request handling
- Layered application architecture
- Hibernate-based database integration
- CRUD-related database operations
- JSP-based user interfaces
- Maven project management

## Author

**Sunil Maske**

- GitHub: https://github.com/Sunilmaske12
- LinkedIn: https://www.linkedin.com/in/sunil-maske/
- LeetCode: https://leetcode.com/u/maskesunil16/
