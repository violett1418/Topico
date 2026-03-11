# Topico API

API REST desarrollada con **Spring Boot** para la gestión de tópicos de un foro.  
Este proyecto fue realizado como parte del **Challenge Foro Hub (Oracle Next Education / Alura)**.


## Tecnologías utilizadas

- Java 23
- Spring Boot
- Spring Security
- JWT (JSON Web Token)
- Spring Data JPA
- Hibernate
- MySQL
- Maven


## Funcionalidades

La API permite realizar operaciones CRUD sobre los tópicos del foro.

Endpoints disponibles:

| Método | Endpoint | Descripción |
|------|------|------|
| POST | `/auth/login` | Autenticación y generación de token JWT |
| GET | `/topicos` | Listar todos los tópicos |
| GET | `/topicos/{id}` | Obtener un tópico por ID |
| POST | `/topicos` | Crear un nuevo tópico |
| PUT | `/topicos/{id}` | Actualizar un tópico |
| DELETE | `/topicos/{id}` | Eliminar un tópico |


## Autenticación

La API utiliza **JWT para proteger los endpoints**.

Después de autenticarse en:

POST /auth/login


se obtiene un token que debe enviarse en los headers:


Authorization: Bearer TU_TOKEN


## Configuración de la base de datos

Ejemplo de configuración en `application.properties`:


spring.datasource.url=jdbc:mysql://localhost:3306/topico
spring.datasource.username=root
spring.datasource.password=tu_contraseña

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true


Proyecto desarrollado por Violett como práctica de aprendizaje en Backend (Spring Boot, API).
