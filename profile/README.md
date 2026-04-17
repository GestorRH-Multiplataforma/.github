# GestorRH - Ecosistema Multiplataforma

Bienvenido a la organización oficial de **GestorRH**. Este ecosistema representa una solución integral y centralizada para la gestión de recursos humanos, automatizando el control de turnos, la tramitación de ausencias y la validación de fichajes mediante tecnologías de geovallado.

![API Version](https://img.shields.io/badge/API-v1.0.1--stable-33cc33?style=flat-square&logo=spring)
![Android Status](https://img.shields.io/badge/Android-en--desarrollo-3DDC84?style=flat-square&logo=android)
![License](https://img.shields.io/badge/license-MIT-yellow?style=flat-square)
![Architecture](https://img.shields.io/badge/Architecture-Clean%20%2B%20MVVM-blue?style=flat-square)

## Hoja de Ruta del Proyecto

El sistema se divide en tres pilares fundamentales, diseñados para trabajar de forma sincronizada bajo un contrato de API robusto:

| Componente | Estado | Tecnología Principal | Propósito |
| :--- | :--- | :--- | :--- |
| [**Backend API**](https://github.com/GestorRH-Multiplataforma/GestorRH-API) | `v1.0.1 Stable` | Java 21 / Spring Boot 3 | Núcleo lógico, seguridad JWT y persistencia de datos. |
| [**Cliente Android**](https://github.com/GestorRH-Multiplataforma/gestorrh-android) | `En Desarrollo` | Kotlin / Jetpack Compose | Interfaz nativa para empleados con validación GPS. |
| **Cliente Escritorio** | `Próximamente` | JavaFX / C# | Gestión administrativa avanzada y reportes complejos. |

## Arquitectura y Estándares de Calidad

Mantenemos un compromiso estricto con la excelencia técnica a través de todo el ecosistema:

* **Clean Architecture & MVVM:** Aplicado tanto en el backend como en el cliente móvil para garantizar la escalabilidad y el desacoplamiento de la lógica de negocio.
* **Seguridad Stateless:** Implementación de autenticación mediante tokens JWT y gestión de sesiones cifradas en el cliente.
* **Persistencia y Resiliencia:** Uso de bases de datos relacionales (PostgreSQL) y sistemas de caché local (Room) para garantizar la disponibilidad de datos incluso sin conexión.
* **Geovallado Inteligente:** Validación de ubicación en tiempo real mediante servicios de localización nativos para asegurar la integridad de los fichajes.

## Metodología de Desarrollo

Nuestra organización opera bajo flujos de trabajo profesionales para asegurar la integridad de la rama principal:

1.  **CI/CD Automatizado:** Cada repositorio cuenta con pipelines (GitHub Actions) que verifican la compilación y ejecutan tests automáticos antes de permitir cambios.
2.  **Norma de Oro:** Prohibición estricta de commits directos a `main`. Todo cambio requiere una *Pull Request* vinculada a su correspondiente *Issue* y aprobada por los checks de calidad.
3.  **Versionado Semántico:** Seguimiento riguroso de **SemVer** para el control de hitos y compatibilidad entre los diferentes clientes y el servidor central.

## Tecnologías Core

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

***
*GestorRH es un proyecto desarrollado con un enfoque en la arquitectura limpia y el despliegue agnóstico a la nube mediante contenedores. Para más información sobre cada componente, visita sus respectivos repositorios.*

