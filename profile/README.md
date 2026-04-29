# GestorRH — Ecosistema Multiplataforma
 
Bienvenido a la organización oficial de **GestorRH**. Este ecosistema representa una solución integral y centralizada para la gestión de recursos humanos, automatizando el control de turnos, la tramitación de ausencias y la validación de fichajes mediante tecnologías de geovallado.
 
![API](https://img.shields.io/badge/API-v1.1.3--stable-brightgreen?style=flat-square&logo=spring)
![Android](https://img.shields.io/badge/Android-v1.0.1--stable-brightgreen?style=flat-square&logo=android)
![Escritorio](https://img.shields.io/badge/Escritorio-en%20desarrollo-orange?style=flat-square&logo=openjdk)
![Architecture](https://img.shields.io/badge/Architecture-Clean%20%2B%20MVVM-blue?style=flat-square)
 
---
 
## Hoja de Ruta del Proyecto
 
El sistema se divide en tres pilares fundamentales, diseñados para trabajar de forma sincronizada bajo un contrato de API robusto:
 
| Componente | Estado | Tecnología Principal | Propósito |
| :--- | :--- | :--- | :--- |
| [**Backend API**](https://github.com/GestorRH-Multiplataforma/GestorRH-API) | `v1.1.3 Stable` | Java 21 / Spring Boot 3 | Núcleo lógico, seguridad JWT y persistencia de datos. |
| [**Cliente Android**](https://github.com/GestorRH-Multiplataforma/gestorrh-android) | `v1.0.1 Stable` | Kotlin / Jetpack Compose | Interfaz nativa para empleados con validación GPS. |
| [**Cliente Escritorio**](https://github.com/GestorRH-Multiplataforma/GestorRH-Escritorio) | `En Desarrollo` | JavaFX 21 | Panel administrativo con reportes y gestión avanzada. |
 
---
 
## Tecnologías Core
 
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![JavaFX](https://img.shields.io/badge/JavaFX-007396?style=for-the-badge&logo=openjdk&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
 
---
 
## Arquitectura del Sistema
 
![Arquitectura del Sistema](./profile/assets/arquitectura_sistema.png)
 
Todos los clientes se comunican exclusivamente con la API REST central mediante tokens JWT, sin acceso directo a la base de datos. Esto garantiza una arquitectura distribuida, segura y agnóstica al cliente.
 
---
 
## Principios Técnicos
 
**Clean Architecture & MVVM** — Aplicado en todos los componentes del ecosistema para garantizar la separación de responsabilidades, la testabilidad y la escalabilidad a largo plazo.
 
**Seguridad Stateless** — Autenticación basada en tokens JWT con gestión de sesiones cifradas en los clientes (EncryptedSharedPreferences en Android, interceptores en JavaFX) y renovación automática ante expiración.
 
**Geovallado Inteligente** — Validación de ubicación GPS en tiempo real mediante `FusedLocationProviderClient` para garantizar la integridad de los fichajes presenciales dentro del radio configurado por la empresa.
 
**Persistencia y Resiliencia** — Estrategia offline-first en el cliente móvil mediante Room Database, permitiendo la consulta de datos sin conexión y sincronización en background al recuperar la red.
 
**Multi-tenant** — La API implementa aislamiento estricto de datos por empresa, garantizando que cada organización solo acceda a su propia información independientemente del volumen de clientes.
 
---
 
## Documentación
 
| Recurso | Descripción |
| :--- | :--- |
| [**Portal de Documentación**](https://gestorrh-multiplataforma.github.io/GestorRH-API/) | Swagger UI interactivo + Javadoc. Desplegado automáticamente vía CI/CD en GitHub Pages. |
| [**README — Backend API**](https://github.com/GestorRH-Multiplataforma/GestorRH-API#readme) | Guía completa de despliegue, variables de entorno, tests y versionado de la API. |
| [**README — Cliente Android**](https://github.com/GestorRH-Multiplataforma/gestorrh-android#readme) | Configuración del entorno, arquitectura y roadmap del cliente móvil. |
| [**README — Cliente Escritorio**](https://github.com/GestorRH-Multiplataforma/GestorRH-Escritorio#readme) | Estado del proyecto, roadmap por épicas y guía de instalación del cliente de escritorio. |
| [**Descarga APK Android**](https://gestorrh-multiplataforma.github.io/github.io/) | Página de descarga del cliente Android con la última versión estable disponible. |
 
---
 
## Metodología de Desarrollo
 
**CI/CD Automatizado** — Cada repositorio dispone de su propio pipeline en GitHub Actions que verifica la compilación y ejecuta la suite de tests automáticamente ante cualquier push o Pull Request.
 
**Norma de Oro** — Prohibición estricta de commits directos a `main`. Todo cambio requiere una Pull Request vinculada a su issue correspondiente y la superación de los Status Checks de CI.
 
**Versionado Semántico** — Seguimiento riguroso de SemVer (`MAJOR.MINOR.PATCH`) para el control de hitos y la garantía de compatibilidad entre clientes y servidor.
 
---
 
*Para más información sobre cada componente, visita sus respectivos repositorios enlazados en la tabla de hoja de ruta.*
