# Student Management System

A robust and secure Student Management System built using **Spring Boot**. This application provides a comprehensive solution for managing students, courses, and course enrollments, complete with an administrative dashboard and secure authentication.

## 🚀 Features

*   **Secure Authentication:** Secure login system implemented using Spring Security to protect administrative routes.
*   **Dashboard:** An interactive dashboard providing an overview of system metrics (e.g., total students, total courses, recent activity).
*   **Student Management:** Complete CRUD (Create, Read, Update, Delete) functionality for managing student records.
*   **Course Management:** Ability to add, edit, view, and remove courses.
*   **Enrollment System:** Seamlessly enroll students into specific courses and manage their enrollments.
*   **Responsive UI:** Frontend interfaces designed with Thymeleaf for dynamic rendering, providing a clean and intuitive user experience.

## 🛠️ Technology Stack

*   **Backend:** Java 21, Spring Boot (Spring MVC, Spring Data JPA, Spring Security)
*   **Frontend:** Thymeleaf (Server-side rendering), HTML/CSS
*   **Database:** MySQL
*   **Data Mapping:** ModelMapper
*   **Build Tool:** Maven

## 📋 Prerequisites

Before you begin, ensure you have the following installed on your machine:
*   [Java Development Kit (JDK) 21](https://www.oracle.com/java/technologies/javase/jdk21-archive-downloads.html) or higher
*   [Maven](https://maven.apache.org/install.html) (Optional, wrapper is included)
*   [MySQL Server](https://dev.mysql.com/downloads/installer/)

## ⚙️ Setup and Installation

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/your-username/student-management-system.git
    cd student-management-system
    ```

2.  **Database Configuration:**
    *   Ensure your local MySQL server is up and running.
    *   The application is configured to automatically create the database `student_mgmt_db` if it doesn't exist.
    *   Open `studentmanagement/src/main/resources/application.properties` and verify/update your MySQL credentials:
        ```properties
        spring.datasource.url=jdbc:mysql://localhost:3306/student_mgmt_db?createDatabaseIfNotExist=true&serverTimezone=UTC
        spring.datasource.username=root
        spring.datasource.password=root
        ```

3.  **Build and Run the Application:**
    Navigate to the `studentmanagement` directory and run the application using the Maven wrapper:
    ```bash
    cd studentmanagement
    ./mvnw spring-boot:run
    ```
    *(On Windows, use `mvnw.cmd spring-boot:run`)*

4.  **Access the Application:**
    *   Open your web browser and navigate to: `http://localhost:8080/`
    *   You will be redirected to the login page. Use the following default admin credentials:
        *   **Username:** `Admin`
        *   **Password:** `admin@123`

## 📂 Project Structure

*   `studentmanagement/`: Contains the main Spring Boot backend code.
    *   `src/main/java/com/cwm/studentmanagement/`: Core Java source code (Controllers, Services, Repositories, Models, Configs).
    *   `src/main/resources/`: Configuration files (`application.properties`) and Thymeleaf templates (`templates/`).
*   `student_management_template/`: Contains static HTML template files used as a reference for the Thymeleaf views.

## 📄 License

This project is licensed under the MIT License. Copyright (c) 2026 Kishan Ojha
