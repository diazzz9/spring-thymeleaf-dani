# Spring Boot + Thymeleaf Starter

Server-side rendered web app built with **Spring Boot 3.5** and **Thymeleaf** (Java 21). A `@Controller` injects data into the model and Thymeleaf renders it into HTML — the foundation for MVC web apps without a separate frontend.

## Stack

Java 21 · Spring Boot 3.5 (Web, Thymeleaf, Actuator, DevTools) · Maven

## Structure

```
src/main
├── java/co/javeriana/dw/thymeleaf
│   ├── ThymeleafApplication.java   → entry point
│   └── HomeController.java         → GET "/" → adds "mensaje" to the model
└── resources/templates/home.html   → renders ${mensaje}
```

## Run

```bash
./mvnw spring-boot:run
```

Open `http://localhost:8080`. Health check via Actuator: `http://localhost:8080/actuator/health`.
