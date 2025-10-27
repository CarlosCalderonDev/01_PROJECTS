
# TECHNOLOGY_STACK

| Categoría                     | Tecnología / Herramienta | Rol dentro del proyecto                                                                                                                               |
| ----------------------------- | ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Framework & Runtime**       | **Axum**                 | Gestiona el enrutamiento, controladores y respuestas HTTP del backend. Es la base sobre la cual se construyen todos los servicios del sistema.        |
|                               | **Tokio**                | Permite que el servidor maneje múltiples solicitudes simultáneamente sin bloquear procesos, garantizando alto rendimiento y baja latencia.            |
| **Base de Datos**             | **PostgreSQL**           | Almacena de forma estructurada la información crítica del sistema: usuarios, procesos, logs y configuraciones. Es el núcleo de persistencia de datos. |
|                               | **SQLx**                 | Actúa como el puente entre el código y la base de datos. Verifica en tiempo de compilación las consultas y asegura integridad en cada transacción.    |
| **Autenticación y Seguridad** | **PASETO**               | Protege los tokens de sesión internos del sistema, asegurando autenticación confiable y libre de vulnerabilidades comunes.                            |
|                               | **JWT (JSON Web Token)** | Gestiona la autenticación entre servicios externos o integraciones de terceros, facilitando comunicación segura entre sistemas.                       |
|                               | **Argon2**               | Se utiliza para proteger las contraseñas de los usuarios y garantizar que los datos sensibles permanezcan inaccesibles ante brechas.                  |
|                               | **rustls**               | Garantiza que toda comunicación HTTP se realice mediante conexiones cifradas (HTTPS), fortaleciendo la privacidad de las transacciones.               |
| **Testing y Calidad**         | **cargo test**           | Automatiza la validación de módulos y funciones del sistema para evitar regresiones durante el desarrollo.                                            |
|                               | **reqwest**              | Simula peticiones reales a los endpoints para validar la funcionalidad del backend bajo distintos escenarios.                                         |
|                               | **tracing**              | Centraliza los logs de ejecución, permitiendo rastrear la actividad del sistema y detectar errores en tiempo real.                                    |
|                               | **metrics**              | Registra estadísticas de rendimiento (latencia, throughput, errores), fundamentales para la observabilidad del proyecto.                              |
|                               | **clippy**               | Asegura que el código siga las buenas prácticas del lenguaje, reduciendo errores y mejorando mantenibilidad.                                          |
|                               | **rustfmt**              | Mantiene un formato uniforme de código, lo que facilita la revisión y colaboración entre desarrolladores.                                             |
|                               | **tarpaulin**            | Mide la cobertura de pruebas para garantizar que las áreas críticas del proyecto estén correctamente validadas.                                       |
|                               | **audit**                | Supervisa las dependencias del proyecto, alertando sobre librerías con fallos de seguridad o versiones obsoletas.                                     |
| **Infraestructura**           | **Docker**               | Estandariza el entorno de ejecución, permitiendo desplegar el proyecto en cualquier servidor sin inconsistencias.                                     |
|                               | **sqlx migrate**         | Administra las migraciones de la base de datos, asegurando que los cambios en el modelo se apliquen de forma controlada.                              |
|                               | **anyhow**               | Simplifica la gestión de errores en producción, capturando fallos inesperados y mejorando la estabilidad general del sistema.                         |
|                               | **thiserror**            | Define errores personalizados y legibles para cada módulo, facilitando el diagnóstico durante el desarrollo y testing.                                |

---

#### TECHNOLOGY_STACK_SUMMARY

| Categoría               | Tecnologías / Herramientas                                                   | Descripción                                           |
| ----------------------- | ---------------------------------------------------------------------------- | ----------------------------------------------------- |
| **Framework & Runtime** | Axum, Tokio                                                                  | Backend asíncrono con alto rendimiento.               |
| **Base de Datos**       | PostgreSQL, SQLx                                                             | Motor SQL confiable con queries tipadas.              |
| **Autenticación**       | PASETO, JWT, Argon2, rustls                                                  | Seguridad híbrida con cifrado moderno.                |
| **Testing & Calidad**   | cargo test, reqwest, tracing, metrics, clippy, rustfmt, tarpaulin, audit     | Integración, observabilidad y auditorías automáticas. |
| **Infraestructura**     | Docker, sqlx migrate, anyhow, thiserror                                      | Despliegue reproducible y manejo robusto de errores.  |

---

#### TECHNOLOGY_STACK_DETAILS

#### 🧱 **2. Versión tipo “Panel de Proyecto” (secciones con íconos y visual jerárquico)**

> Ideal para mostrarlo en Notion, una Wiki o documentación técnica web.

---

#### 🧩 Framework y Runtime

**Axum** + **Tokio**

> Base del servidor asíncrono de alto rendimiento.

---

#### 🗄️ Base de Datos

**PostgreSQL** con **SQLx**

> Consultas tipadas y seguras en tiempo de compilación.

---

#### 🔐 Autenticación y Seguridad

> * **PASETO** → interno (seguridad máxima)
> * **JWT** → externo (compatibilidad estándar)
> * **Argon2** → hashing de contraseñas
> * **rustls** → cifrado TLS/HTTPS

---

#### 🧪 Testing y Calidad

> * **Unitarias:** cargo test
> * **Integración:** reqwest
> * **Observabilidad:** tracing, metrics, prometheus
> * **Auditorías:** clippy, rustfmt, tarpaulin, audit

---

#### ⚙️ Infraestructura

> * **Docker:** entornos consistentes
> * **sqlx migrate:** migraciones estructuradas
> * **Errores:** anyhow / thiserror

---

#### 🧭 Principios

> Seguridad · Compatibilidad · Observabilidad · Automatización · Calidad continua

---

#### 📜 **3. Versión “Roadmap Visual” (útil para presentaciones)**

```plaintext
┌──────────────────────────────────────────┐
│      🚀 Stack Tecnológico (Rust API)     │
├──────────────────────────────────────────┤
│ 🧩 Framework      → Axum + Tokio          │
│ 🗄️ Base de Datos  → PostgreSQL + SQLx     │
│ 🔐 Seguridad      → PASETO / JWT / Argon2 │
│ 🧪 Testing        → cargo test / reqwest  │
│ 📊 Observabilidad → tracing / metrics     │
│ ⚙️ Infraestructura → Docker / sqlx migrate │
│ 💡 Principios     → Seguridad / Calidad   │
└──────────────────────────────────────────┘
```

---

#### 📘 Nota del Autor

> Este stack tecnológico ha sido seleccionado no solo en función de las necesidades actuales del proyecto, sino también como parte de un propósito de aprendizaje y consolidación profesional en el ecosistema de **Rust** y sus herramientas asociadas.
> Aunque se reconoce que, en el futuro, podrían realizarse ajustes o sustituciones según la evolución del proyecto o las condiciones técnicas que se presenten, **la intención principal es mantener la coherencia tecnológica y el compromiso con este enfoque**.
> El objetivo no es únicamente construir una API eficiente y moderna, sino también fortalecer la experiencia práctica con las tecnologías aquí empleadas.