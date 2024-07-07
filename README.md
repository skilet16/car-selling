# Car-Selling

This project is a car selling web application where users can register, log in, add their cars for sale, and view available cars to buy on the home page.

## Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Setup](#setup)
  - [Backend Setup](#backend-setup)
  - [Frontend Setup](#frontend-setup)
- [Running the Project](#running-the-project)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## Introduction
This project is a car selling web application where users can register, log in, add their cars for sale, and view available cars to buy on the home page.

## Prerequisites
Before you begin, ensure you have the following installed:
- [Java Development Kit (JDK) 11+](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html)
- [Apache Maven](https://maven.apache.org/install.html)
- [PostgreSQL](https://www.postgresql.org/download/)
- [Node.js and npm](https://nodejs.org/)

## Setup

### Backend Setup
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/corvantaanalytics/car-selling.git
    cd car-selling
    ```

2. **Install Maven**:
    Follow the instructions [here](https://maven.apache.org/install.html) to install Maven on your system.

3. **Setup PostgreSQL**:
    - Install and run PostgreSQL.
    - Create a new database:
      ```sql
      CREATE DATABASE your_database_name;
      ```

4. **Configure Database**:
    Create a file named `application.properties` in `src/main/resources` and add your database configuration:
    ```properties
    spring.datasource.url=jdbc:postgresql://localhost:5432/your_database_name
    spring.datasource.username=your_db_username
    spring.datasource.password=your_db_password
    spring.jpa.generate-ddl=true
    ```

5. **Build and Run the Backend**:
    ```bash
    mvn install
    mvn spring-boot:run
    ```

### Frontend Setup
1. **Navigate to the Frontend Directory**:
    ```bash
    cd frontend
    ```

2. **Install Dependencies**:
    ```bash
    npm install
    ```

3. **Run the Frontend**:
    ```bash
    npm start
    ```

## Running the Project
After setting up both backend and frontend, you can access the application at `http://localhost:3000` for the frontend and `http://localhost:8080` for the backend.

## Project Structure

### Backend (Spring Boot)
- `src/main/java`: Contains Java source files.
- `src/main/resources`: Contains application configuration files.
- `pom.xml`: Maven configuration file.

### Frontend (React)
- `frontend/src`: Contains React components and Redux-related files.
- `frontend/public`: Public assets.
- `package.json`: Node.js project configuration file.

## Technologies Used
- **Backend**: Spring Boot, JPA, PostgreSQL
- **Frontend**: React, Redux
- **Build Tools**: Maven (for backend), npm (for frontend)

## Contributing
We welcome contributions to enhance this project. Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature-name`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/your-feature-name`).
6. Create a new Pull Request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
