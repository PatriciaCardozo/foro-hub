# foro-hub
API REST de Foro Hub para gestionar tópicos
# ForoHub - API REST de Tópicos

ForoHub es una API REST desarrollada en Java con Spring Boot que permite gestionar tópicos en un foro, ofreciendo funcionalidades de creación, consulta, actualización y eliminación de tópicos. El proyecto incluye autenticación básica y JWT para proteger el acceso a la API.

## Funcionalidades principales

- Crear un nuevo tópico (POST `/topicos`)
- Listar todos los tópicos (GET `/topicos`)
- Consultar un tópico específico por ID (GET `/topicos/{id}`)
- Actualizar un tópico (PUT `/topicos/{id}`)
- Eliminar un tópico (DELETE `/topicos/{id}`)
- Gestión de usuarios y autenticación con JWT
- Validaciones de datos y reglas de negocio (campos obligatorios, evitar duplicados)

## Tecnologías utilizadas

- Java 17+
- Spring Boot 3+
- Spring Web
- Spring Data JPA
- Spring Security
- JWT (JSON Web Token)
- MySQL
- Maven
- Flyway (migraciones de base de datos)
- Lombok (para reducir código repetitivo)

## Estructura del proyecto

## Endpoints de ejemplo

| Método | Endpoint               | Descripción                        |
|--------|-----------------------|------------------------------------|
| POST   | `/topicos`            | Crear un nuevo tópico               |
| GET    | `/topicos`            | Listar todos los tópicos            |
| GET    | `/topicos/{id}`       | Consultar un tópico por ID          |
| PUT    | `/topicos/{id}`       | Actualizar un tópico existente      |
| DELETE | `/topicos/{id}`       | Eliminar un tópico por ID           |
| POST   | `/login`              | Autenticación de usuario (JWT)      |

>  Nota: Este proyecto se puede ejecutar en local y conectarse a una base de datos MySQL. Para la autenticación JWT, se requiere definir `jwt.secret` y `jwt.expiration` en `application.properties`.

## Cómo usar

1. Clonar el repositorio:  
```bash
git clone <URL_DE_TU_REPOSITORIO>
