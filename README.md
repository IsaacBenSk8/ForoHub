# ForoHub

Bienvenido a ForoHub, una API REST diseñada para un foro y desarrollada con Spring Boot. Este proyecto forma parte del desafío final del curso Practicando Spring Framework: Challenge Foro Hub. La aplicación permite a los usuarios registrarse, iniciar sesión, crear tópicos y responder a ellos, todo ello gestionado de forma segura mediante autenticación JWT.

## Índice

- [Características](#características)
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Requisitos Previos](#requisitos-previos)
- [Configuración](#configuración)
- [Endpoints](#endpoints)
- [Contribución](#contribución)
- [Autor](#autor)
- [Licencia](#licencia)

## Características

- Registro y autenticación de usuarios.
- Creación y gestión de tópicos.
- Autenticación segura con JWT.
- Endpoints protegidos.
- Documentación API con Swagger.

## Tecnologías Utilizadas

- Java 17
- Spring Boot
- Spring Security
- JWT (JSON Web Tokens)
- JPA (Java Persistence API)
- Hibernate
- MySQL
- Lombok
- Flyway
- Swagger

## Requisitos Previos

- Java 17
- Maven
- MySQL

# Configuración

Para configurar la base de datos MySQL, actualiza el archivo `application.properties` con tus credenciales:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/forohub
spring.datasource.username=root
spring.datasource.password=root1234
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

spring.h2.console.enabled=true

jwt.secret=mysecretkey
jwt.expiration=86400000
```
## Endpoints
- POST /users: Registra un nuevo usuario.
- POST /login: Inicia sesión y recibe un token JWT.
- POST /topics: Crea un nuevo tópico.
- GET /topics: Muestra una lista de todos los tópicos.
- DELETE /topics/{id}: Elimina un tópico por su ID.

## Autor
Isaac Flores