# Parking Control API

## 📌 Project Overview
The **Parking Control API** is a RESTful web service built with **Spring Boot** that provides parking spot management functionality. It allows users to create, read, update and delete parking spots using standard HTTP methods.

### 🛠 Technologies Used
- **Spring Boot**: Bootstraps the application and provides an embedded Tomcat server.
- **Spring MVC**: Enables the development of the web layer.
- **Spring Data JPA**: Facilitates database interactions with PostgreSQL.
- **Spring Validation**: Provides basic validation for request payloads.
- **PostgreSQL**: Relational database used for persistent storage.

### 🚀 API Endpoints
| Method | Endpoint                | Description |
|--------|-------------------------|-------------|
| GET    | `/parking-spot`        | Retrieve a paginated list of parking spots. |
| GET    | `/parking-spot/{id}`    | Retrieve a specific parking spot by ID. |
| POST   | `/parking-spot`        | Create a new parking spot. |
| PUT    | `/parking-spot/{id}`    | Update an existing parking spot. |
| DELETE | `/parking-spot/{id}`    | Delete a parking spot by ID. |

---

## 🏗 Understanding Spring Boot and the Spring Framework

### 🔹 Spring Framework
Spring is a powerful Java framework designed to simplify enterprise application development. It is structured into **seven core modules**:
- **Data Access/Integration**: Handles database interactions.
- **Web**: Provides web-related functionality, including Spring MVC.
- **AOP (Aspect-Oriented Programming)**: Enables modularization of cross-cutting concerns.
- **Aspects**: Implements aspect-oriented programming features.
- **Instrumentation**: Supports Java instrumentation for monitoring and profiling.
- **Messaging**: Facilitates message-based communication.
- **Core Container**: Provides the fundamental IoC (Inversion of Control) and dependency injection capabilities.

### 🔹 Key Spring Concepts
- **Inversion of Control (IoC)**: A design principle where objects declare their dependencies instead of creating them, delegating their instantiation to the Spring IoC container.
- **Dependency Injection (DI)**: A mechanism to implement IoC by injecting required dependencies into objects at runtime.
- **Bean**: Any object managed by the Spring container. Beans are instantiated, assembled, and controlled by Spring using IoC and DI.
- **Spring Stereotypes**:
  - `@Component`: Generic stereotype for a Spring-managed component.
  - `@Service`: Indicates a service layer component.
  - `@Repository`: Represents a persistence layer component.
  - `@Controller`: Defines a web controller in an MVC architecture.

### 🔹 Spring Boot
Spring Boot is a project within the Spring ecosystem that simplifies application development by removing boilerplate configurations. It provides:
- **Embedded server** (Tomcat or Netty) – eliminating the need for external deployment.
- **Automatic configuration** – reducing manual setup and XML configuration.
- **Spring Boot Starters** – predefined dependencies to streamline project setup.

When a Spring Boot application starts, an embedded **Tomcat server** runs on **port 8080** (default) in the case of an MVC project.

---

## ⚡ How to Run the Application
### Prerequisites
- JDK 11+
- PostgreSQL database
- Maven

### Running Locally
1. Clone the repository:
   ```sh
   git clone https://github.com/gabrielgatti7/Parking-Control-Spring-Boot.git
   cd Parking-Control-Spring-Boot
   ```
2. Configure the database settings in `src/main/resources/application.properties`.
3. Build and run the application:
   ```sh
   mvn spring-boot:run
   ```
4. The API will be available at:
   ```sh
   http://localhost:8080/parking-spot
   ```

---

## 📜 License
This project is for educational purposes. Feel free to modify and use it as needed!

---

## 📩 Contact
For any questions or suggestions, feel free to reach out!

---

Happy coding! 🚀

