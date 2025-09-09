# Level 1 - Spring and Maven Exercise

📄 **Description - Exercise Statement**

This exercise is an introduction to **Spring** and **Maven**.
The objective is to create a Spring Boot project using [Spring Initializr](https://start.spring.io/) and implement a simple REST API with two methods that return a welcome message.

---

💻 **Technologies Used**

- Java 21
- Spring Boot (latest stable version, 3.x)
- Spring Web
- Spring Boot DevTools
- Maven (dependency manager)
- Eclipse / IntelliJ IDEA (recommended IDE)

---

📋 **Requirements**

- **JDK 21**
- **Maven 3.9+** installed and configured in PATH
- Internet connection to download dependencies
- Configure the port in `application.properties`:
```properties
server.port=9000
```

---

🛠️ **Installation**

1. Access [Spring Initializr](https://start.spring.io/).

2. Generate a project with the following configuration:
- **Project**: Maven
- **Language**: Java
- **Spring Boot**: Latest stable version
- **Group**: `cat.itacademy.s04.t01.n01`
- **Artifact**: `S04T01N01`
- **Name**: `S04T01N01`
- **Description**: `S04T01N01`
- **Package name**: `cat.itacademy.s04.t01.n01`
- **Packaging**: Jar
- **Java**: 21
- **Dependencies**: Spring Boot DevTools, Spring Web

3. Import the project into your editor of choice:

`File > Import > Existing Maven Project`

---

▶️ **Run**

Compile and Run the application with Maven:

```bash
# Compile the project
mvn compile

# Clean the project
mvn clean

# Package the project
mvn package

# Run the application
mvn spring-boot:run
```

The application will be available at:
👉 [http://localhost:9000](http://localhost:9000)

---

🌐 **Deployment**

This project is intended for **local educational use only** and is not intended to be deployed in a production environment.

---

🤝 **Contributions**

Contributions are welcome! To contribute:

1. Fork this repository.
2. Create a branch (`git checkout -b feature/my-feature`).
3. Commit your changes.
4. Push to your branch (`git push origin feature/my-feature`).
5. Open a Pull Request.

---

## 📡 **Available endpoints**

### 1️⃣API HelloWorld 

**GET /HelloWorld**
````
Response:
Hello, UNKNOWN. You are running a Maven project
````

**GET /HelloWorld?name=MyName**
```
Response:
Hello, MyName. You are running a Maven project
```

### 2️⃣API HelloWorld2
```http
GET /HelloWorld2
GET /HelloWorld2/MyName
```

**GET /HelloWorld2**
```
Hello, UNKNOWN. You are running a Maven project.
```
**GET /HelloWorld2/MyName**
```
Hello, MyName. You are running a Maven project.
```

---

✍️ **Author**
Exercise completed as part of **Sprint 4 - IT Academy**.