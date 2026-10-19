# Osama Khalili

**Java Backend Developer** — REST APIs, layered architecture, relational persistence, and CI/CD.

I build maintainable server-side applications with Java and Spring Boot, and I care about clean separation of concerns, meaningful error handling, and tests that actually verify behavior. My work spans Java EE (JAX-RS/JPA/CDI), Spring Boot REST and MVC applications, JavaFX desktop apps, and full-stack JavaScript/TypeScript.

---

## Tech Stack

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Hibernate](https://img.shields.io/badge/JPA_/_Hibernate-59666C?style=flat-square&logo=hibernate&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white)
![JUnit 5](https://img.shields.io/badge/JUnit_5-25A162?style=flat-square&logo=junit5&logoColor=white)
![REST](https://img.shields.io/badge/REST_APIs-005571?style=flat-square&logo=fastapi&logoColor=white)
![JavaFX](https://img.shields.io/badge/JavaFX-FF6600?style=flat-square&logo=openjdk&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

**Core:** Java 11/16, Spring Boot, Spring Data JPA, Hibernate, JAX-RS, CDI, JPA, Thymeleaf, Maven, JUnit 5, Mockito
**Infrastructure:** Docker, Jenkins pipelines, Maven build lifecycle, WildFly / application servers
**Frontend:** Next.js, React, TypeScript, JavaScript, HTML5, CSS3, Thymeleaf templates
**Data:** MySQL, relational modelling, JSON data pipelines

---

## Featured Projects

### [student-management-system](https://github.com/osamakhalili/student-management-system)
Java EE REST API built with **JAX-RS + JPA + CDI** and packaged as a WAR for deployment on an application server.
- Full CRUD surface: `GET`, `POST`, `PUT`, `PATCH`, `DELETE` plus lookup by last name
- Layered design: `entity` → `service` → `rest`, with a dedicated `JAXRSConfiguration` and `persistence.xml`
- Email uniqueness enforced at the persistence layer and translated into explicit HTTP responses
- Consistent error contracts: `404` with descriptive plain-text bodies instead of stack traces
- Built in a two-person team; documented every endpoint and payload in the README

**Stack:** `Java` `JAX-RS` `JPA` `CDI` `Maven` `WildFly`

---

### [book](https://github.com/osamakhalili/book)
A complete bookstore split into a **Spring Boot REST backend** and a **vanilla JavaScript frontend**.
- `BookController` exposes list, by-id, create, update, and delete endpoints under `/book`
- Constructor injection with a service layer on top of a `JpaRepository`
- `@CrossOrigin` configuration so the static frontend can consume the API directly
- Custom `UserNotFoundException` mapped to a clean API error
- Frontend ships a customer catalog (`index.html`) and an admin panel (`admin.html`) with their own CSS/JS

**Stack:** `Java` `Spring Boot` `Spring Data JPA` `REST` `JavaScript` `HTML/CSS`

---

### [pizzaApp2](https://github.com/osamakhalili/pizzaApp2) · [PizzaApp](https://github.com/osamakhalili/PizzaApp)
The same domain implemented twice, which is exactly why it is useful: first as a REST API, then as a server-rendered application.
- **PizzaApp:** Spring Boot REST service with controller/service/repository layers and `PATCH` support for partial updates
- **pizzaApp2:** Spring MVC + Thymeleaf with `index`, `new_pizza`, and `update_pizza` views backed by the same CRUD model
- Both use Spring Data JPA persistence and Maven builds

**Stack:** `Java` `Spring Boot` `Spring MVC` `Thymeleaf` `JPA` `Maven`

---

### [GameOfLife2](https://github.com/osamakhalili/GameOfLife2)
Conway's Game of Life as a **JavaFX desktop application** with an explicit MVC split.
- `Grid` and `GridCell` hold the simulation state and neighbour logic, independent of the UI
- `AppController` binds the model to the FXML view; `App` handles application startup
- Java modules (`module-info.java`) and a Maven build with JavaFX, FormsFX, and TilesFX dependencies
- Unit tests for the grid rules with JUnit 4

**Stack:** `Java` `JavaFX` `FXML` `Maven` `JUnit`

---

### [mobile-project1](https://github.com/osamakhalili/mobile-project1)
A Maven application wired into a **complete CI/CD pipeline** — the project where build automation was the point.
- `Jenkinsfile` with staged pipeline: checkout → compile → `mvn verify` / `mvn test` → package → Docker build → Docker Hub push
- Dockerfile based on `adoptopenjdk:16-jre`, exposing the application port and running the packaged JAR
- Unit tests with JUnit 5 and Mockito
- Demonstrates the full path from commit to published container image

**Stack:** `Java` `Maven` `Jenkins` `Docker` `JUnit 5` `Mockito`

---

### [java_lab2](https://github.com/osamakhalili/java_lab2)
A **test-driven** String Calculator kata, written test-first with JUnit 5.
- Handles empty input, single and multiple numbers, whitespace, and newline separators
- Configurable delimiters, including multi-character delimiters
- Rejects negative numbers with a descriptive exception listing every offending value
- Ignores values above 1000, matching the kata specification
- Fifteen tests, each named with `@DisplayName` for the behaviour it proves

**Stack:** `Java` `JUnit 5` `TDD`

---

## Additional Experience

**Driving-Theory Question Bank (data engineering & content pipeline)**
Built and maintained a structured question bank for Swedish driving-licence theory (taxi, bus, truck, and professional competence categories).
- **4,651 questions** across **15 category datasets** and **112 distinct quizzes**
- Bilingual content model: Swedish and Arabic variants with a shared schema
- **1,853 questions with images** and **2,508 with audio**, with media references resolved into a consistent local asset store
- Normalised JSON schema (`questionNumber`, `answers[]`, `correctAnswer`, `imageUrl`, `audioUrl`, `quizUrl`) designed for direct consumption by a quiz client
- Worked through encoding, duplicate-question, and broken-media issues to produce clean, importable datasets

---

## GitHub Activity

<p>
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=osamakhalili&show_icons=true&hide_border=true&count_private=true" alt="GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=osamakhalili&layout=compact&hide_border=true&langs_count=6" alt="Top languages" />
</p>

---

## Focus Areas

- Backend design with clear controller / service / repository boundaries
- REST contract quality: correct status codes, predictable payloads, useful error messages
- Persistence modelling with JPA and Hibernate
- Test-driven development and automated build pipelines
- Containerised delivery from source to registry

---

<sub>Java backend developer based in Sweden. Open to backend and full-stack opportunities.</sub>
