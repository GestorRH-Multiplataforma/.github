# GestorRH - Ecosistema Multiplataforma

Bienvenido a la organización principal de **GestorRH**, un sistema centralizado e integral para la gestión de recursos humanos, control de turnos, ausencias y validación de fichajes con geovallado.

## Nuestra Arquitectura

Este proyecto está diseñado bajo una arquitectura cliente-servidor robusta, priorizando la seguridad, la escalabilidad y la facilidad de despliegue.

### Backend Core (Desarrollado y Estable)
El corazón del sistema es una API RESTful sólida y segura.
* **Tecnología:** Java, Spring Boot, Spring Security (JWT)
* **Base de Datos:** PostgreSQL
* **Infraestructura:** Completamente dockerizado (Docker & Docker Compose) para entornos de desarrollo y producción.
* [Ver Repositorio de la API](https://github.com/GestorRH-Multiplataforma/GestorRH-API)

### Clientes Multiplataforma (En Desarrollo / Próximamente)
Consumiendo los endpoints de nuestra API central, el ecosistema se expandirá con interfaces nativas:
* **Android:** Desarrollo nativo en Kotlin.
* **Escritorio:** Aplicación de gestión administrativa en JavaFX.

## 🛠️ Tecnologías y Herramientas

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-0095D5?style=for-the-badge&logo=kotlin&logoColor=white)

---
*Organización mantenida y desarrollada aplicando metodologías de CI/CD, Conventional Commits y entornos aislados.*
