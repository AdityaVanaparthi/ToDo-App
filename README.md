# ToDo Application

A simple task management web application built using Java, Spring Boot, Spring Data JPA, MySQL, and Thymeleaf. It allows users to create tasks, view their task list, mark tasks as completed, and delete tasks.

## Features

- **Add Tasks:** Create new tasks using the input form.
- **View Tasks:** Display all saved tasks.
- **Mark as Completed:** Toggle a task between completed and pending.
- **Delete Tasks:** Remove tasks from the list.
- **Database Persistence:** Store tasks in a MySQL database.
- **Responsive UI:** A dark-themed interface with orange and blue visual indicators.

## Technologies Used

- Java
- Spring Boot
- Spring MVC
- Spring Data JPA
- MySQL
- Thymeleaf
- HTML and CSS
- Maven
- JUnit 5

## Project Structure

```text
todoapp/
├── src/
│   ├── main/
│   │   ├── java/com/app/todoapp/
│   │   │   ├── controller/
│   │   │   │   └── TaskController.java
│   │   │   ├── model/
│   │   │   │   └── Task.java
│   │   │   ├── repository/
│   │   │   │   └── TaskRepository.java
│   │   │   ├── service/
│   │   │   │   └── TaskService.java
│   │   │   └── TodoappApplication.java
│   │   └── resources/
│   │       ├── templates/
│   │       │   └── tasks.html
│   │       └── application.properties
│   └── test/
├── pom.xml
└── mvnw
```

## Prerequisites

Install the following before running the application:

- Java JDK
- MySQL Server
- Maven (optional if using the included Maven Wrapper)

## Database Configuration

1. Start your MySQL server.
2. Create the database:

```sql
CREATE DATABASE `todo-app`;
```

3. Configure the following environment variables:

| Variable | Example |
|---|---|
| `DB_URL` | `jdbc:mysql://localhost:3306/todo-app` |
| `DB_USERNAME` | `root` |
| `DB_PASSWORD` | Your MySQL password |

Do not commit real passwords or credentials to GitHub.

## Run the Application

From the `todoapp` project directory, run the following command on Windows:

```bash
mvnw.cmd spring-boot:run
```

Alternatively, use Maven if it is installed:

```bash
mvn spring-boot:run
```

Open your browser and visit:

http://localhost:8080/

## Testing

Run the tests using the Maven Wrapper on Windows:

```bash
mvnw.cmd test
```

## Future Improvements

- Add user authentication and authorization.
- Add task due dates and priorities.
- Add input validation and improved error handling.
- Add automated tests for task operations.

## Author

**Aditya Vanaparthi**

GitHub: [AdityaVanaparthi](https://github.com/AdityaVanaparthi)
