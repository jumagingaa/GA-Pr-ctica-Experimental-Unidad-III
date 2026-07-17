#  Sistema Integrado de Gestión de Biblioteca con Código QR (SIGCB-QR)

## Descripción

SIGCB-QR es un sistema web desarrollado para optimizar la administración de una biblioteca mediante el uso de códigos QR. La aplicación permite gestionar usuarios, libros, ejemplares y préstamos, incorporando mecanismos modernos de autenticación y control de sesiones mediante JSON Web Tokens (JWT) y Redis.

El sistema está diseñado bajo una arquitectura cliente-servidor utilizando Angular para el frontend y Spring Boot para el backend, con PostgreSQL como base de datos principal.

---

# Objetivos

- Automatizar la gestión de préstamos y devoluciones.
- Administrar usuarios, libros y categorías.
- Implementar autenticación segura mediante JWT.
- Gestionar sesiones utilizando Redis.
- Generar códigos QR para identificar ejemplares.
- Mejorar la seguridad mediante cookies HttpOnly.

---

# Tecnologías utilizadas

### Backend

- Java 21
- Spring Boot 3
- Spring Security
- Spring Data JPA
- JWT
- Redis
- Maven

### Frontend

- Angular

### Base de Datos

- PostgreSQL
- Redis

### Herramientas

- IntelliJ IDEA
- Visual Studio Code
- Git
- GitHub
- Draw.io
- PlantUML

---

# Arquitectura del sistema

El proyecto implementa una arquitectura multicapa compuesta por:

- Frontend (Angular)
- API REST (Spring Boot)
- Capa de Servicios
- Capa de Repositorios
- PostgreSQL
- Redis

---

# Funcionalidades principales

- Inicio de sesión seguro.
- Autenticación mediante JWT.
- Almacenamiento del token en Cookie HttpOnly.
- Gestión de usuarios.
- Gestión de roles.
- Gestión de categorías.
- Gestión de libros.
- Gestión de ejemplares.
- Registro de préstamos.
- Registro de devoluciones.
- Consulta del historial de préstamos.
- Generación de códigos QR.
- Revocación de sesiones utilizando Redis.

---

# Seguridad implementada

El sistema incorpora diversas medidas de seguridad:

- Autenticación mediante JSON Web Token (JWT).
- Cookies HttpOnly para proteger el token.
- Contraseñas cifradas con BCrypt.
- Spring Security.
- Control de acceso por roles.
- Redis para administrar la revocación de tokens.
- Protección de endpoints mediante filtros JWT.

---

# Diagramas desarrollados

Durante el desarrollo se elaboró la siguiente documentación técnica:

- Modelo C4 Nivel 1
- Modelo C4 Nivel 2
- Diagrama de Casos de Uso
- Diagrama de Clases
- Diagrama de Secuencia
- Modelo Entidad-Relación
- Flujo de autenticación JWT
- Proceso de autenticación utilizando JWT y Redis
- Arquitectura del sistema

---

# Rendimiento

Se realizó una comparación entre PostgreSQL y Redis.

## PostgreSQL

- Persistencia de datos.
- Integridad referencial.
- Consultas SQL.
- Almacenamiento permanente.

## Redis

- Almacenamiento en memoria.
- Baja latencia.
- Gestión rápida de sesiones.
- Revocación inmediata de tokens JWT.
- Alto rendimiento para autenticación.

---

# Estructura del proyecto

```
SIGCB-QR
│
├── backend
│   ├── controller
│   ├── service
│   ├── repository
│   ├── entity
│   ├── dto
│   ├── security
│   └── config
│
├── frontend
│
├── imagenes
│
└── README.md
```

---

# Requisitos

- Java 21
- Maven
- PostgreSQL
- Redis
- Node.js
- Angular CLI

---

# Ejecución

## Backend

```bash
mvn clean install
mvn spring-boot:run
```

## Frontend

```bash
npm install
ng serve
```

---

# Principales beneficios

- Arquitectura escalable.
- Código organizado por capas.
- Seguridad basada en JWT.
- Integración con Redis.
- Persistencia segura con PostgreSQL.
- Fácil mantenimiento.
- Documentación UML completa.

---

# Autores

- Jefferson Manuel Umaginga Arevalo
- Ayala Ormaza Janeth Nataly
- Kevin Moisés Castro Espinoza
- Erick Jhair Mera Arias
- Ricardo Elías Vélez López

---

# Licencia

Proyecto desarrollado con fines académicos para la Universidad Técnica Estatal de Quevedo (UTEQ).
