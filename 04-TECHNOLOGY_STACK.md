# TECHNOLOGY_STACK

# 💎 **1. Versión tipo “Ficha Técnica” (limpia y elegante)**

| Categoría               | Tecnologías / Herramientas                                                   | Descripción                                           |
| ----------------------- | ---------------------------------------------------------------------------- | ----------------------------------------------------- |
| **Framework & Runtime** | Axum, Tokio                                                                  | Backend asíncrono con alto rendimiento.               |
| **Base de Datos**       | PostgreSQL, SQLx                                                             | Motor SQL confiable con queries tipadas.              |
| **Autenticación**       | PASETO, JWT, Argon2, rustls                                                  | Seguridad híbrida con cifrado moderno.                |
| **Testing & Calidad**   | cargo test, reqwest, tracing, metrics, clippy, rustfmt, tarpaulin, audit     | Integración, observabilidad y auditorías automáticas. |
| **Infraestructura**     | Docker, sqlx migrate, anyhow, thiserror                                      | Despliegue reproducible y manejo robusto de errores.  |
| **Principios Clave**    | Seguridad, Compatibilidad, Observabilidad, Automatización, Pruebas continuas | Guía de diseño y desarrollo del sistema.              |

---

#### 🧱 **2. Versión tipo “Panel de Proyecto” (secciones con íconos y visual jerárquico)**

> Ideal para mostrarlo en Notion, una Wiki o documentación técnica web.

---

#### 🧩 Framework y Runtime

**Axum** + **Tokio**
→ Base del servidor asíncrono de alto rendimiento.

---

#### 🗄️ Base de Datos

**PostgreSQL** con **SQLx**
→ Consultas tipadas y seguras en tiempo de compilación.

---

#### 🔐 Autenticación y Seguridad

* **PASETO** → interno (seguridad máxima)
* **JWT** → externo (compatibilidad estándar)
* **Argon2** → hashing de contraseñas
* **rustls** → cifrado TLS/HTTPS

---

#### 🧪 Testing y Calidad

* **Unitarias:** cargo test
* **Integración:** reqwest
* **Observabilidad:** tracing, metrics, prometheus
* **Auditorías:** clippy, rustfmt, tarpaulin, audit

---

#### ⚙️ Infraestructura

* **Docker:** entornos consistentes
* **sqlx migrate:** migraciones estructuradas
* **Errores:** anyhow / thiserror

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

#### 📘 Nota del Autor

Este stack tecnológico ha sido seleccionado no solo en función de las necesidades actuales del proyecto, sino también como parte de un propósito de aprendizaje y consolidación profesional en el ecosistema de **Rust** y sus herramientas asociadas.

Aunque se reconoce que, en el futuro, podrían realizarse ajustes o sustituciones según la evolución del proyecto o las condiciones técnicas que se presenten, **la intención principal es mantener la coherencia tecnológica y el compromiso con este enfoque**.

El objetivo no es únicamente construir una API eficiente y moderna, sino también fortalecer la experiencia práctica con las tecnologías aquí empleadas.