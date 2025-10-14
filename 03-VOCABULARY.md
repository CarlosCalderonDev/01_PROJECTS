# 03-VOCABULARY

## 1. **Entidades**

* **Usuario**: Cliente, administrador o profesional del servicio.
* **Cita**: Registro con fecha, hora, estado (pendiente, confirmada, cancelada).
* **Servicio**: Tipo de atención (consulta, asesoría, etc.).
* **Recurso**: Profesional, sala o equipo asociado a la cita.
* **Notificación**: Mensajes enviados al cliente (email, SMS, app).

---

## 2. **Reglas de negocio**

* No se pueden agendar dos citas en el mismo horario para el mismo recurso.
* La cita debe estar dentro del horario laboral del recurso.
* Un cliente solo puede cancelar hasta X horas antes de la cita.
* Ciertas citas requieren pago anticipado para confirmarse.
* Notificaciones obligatorias: confirmación, recordatorio, cancelación.

---

## 3. **Procesos de negocio**

* **Agendar cita**: Cliente selecciona servicio → sistema valida disponibilidad → genera cita → envía confirmación.
* **Cancelar cita**: Cliente solicita cancelación → sistema valida plazo permitido → actualiza estado → notifica a todos los involucrados.
* **Reprogramar cita**: Cliente selecciona nuevo horario → sistema valida disponibilidad → actualiza cita → notifica.
* **Recordatorio automático**: Sistema identifica citas próximas → envía notificación al cliente y al recurso.






## 🧠 TERMINOLOGÍA ESENCIAL EN DISEÑO DE SISTEMAS

#### 🔹 Nivel 1: Conceptos básicos

| Término                | Significado                                                              |
| ---------------------- | ------------------------------------------------------------------------ |
| **Entidad**            | Objeto del mundo real o lógico sobre el que guardas datos (ej: Usuario). |
| **Atributo**           | Propiedad de una entidad (ej: `email`, `nombre`, `fecha_nacimiento`).    |
| **Relación**           | Conexión entre dos entidades (ej: un Usuario tiene muchas Citas).        |
| **Módulo**             | Parte del sistema que cumple una función específica (ej: Agenda).        |
| **Función (o Método)** | Acción que ejecuta una entidad o módulo (ej: `crearFactura()`).          |

#### 🔹 Nivel 2: Diseño orientado a objetos / estructuración de código

| Término             | Significado                                                         |
| ------------------- | ------------------------------------------------------------------- |
| **Clase**           | Modelo para crear objetos con atributos y métodos (OOP).            |
| **Objeto**          | Instancia concreta de una clase.                                    |
| **Responsabilidad** | Tarea o función asignada a un módulo o clase.                       |
| **Interfaz**        | Contrato que define métodos sin implementarlos (ej: `Notificable`). |
| **Herencia**        | Permite que una clase derive de otra.                               |
| **Composición**     | Relación donde una clase contiene otras clases como partes.         |

📌 *Aplica en TypeScript, Go (con structs/interfaces), JavaScript, etc.*

---

#### 🔹 Nivel 3: Modelado y arquitectura de sistemas

| Término                        | Significado                                                                  |
| ------------------------------ | ---------------------------------------------------------------------------- |
| **Actor**                      | Entidad externa que interactúa con el sistema (Usuario, Admin, API externa). |
| **Caso de uso**                | Escenario funcional que describe qué hace el sistema (ej: “Emitir factura”). |
| **Componente**                 | Unidad lógica independiente (ej: servicio de correo, módulo de pagos).       |
| **Servicio (Service)**         | Lógica de negocio que cumple una función (ej: `FacturaService`).             |
| **Repositorio (Repository)**   | Abstracción para acceder a datos (ej: `UserRepository` → DB).                |
| **Controlador (Controller)**   | Punto de entrada para recibir solicitudes HTTP.                              |
| **DTO (Data Transfer Object)** | Objeto para transferir datos entre capas o servicios.                        |
| **Middleware**                 | Componente que intercepta peticiones/respuestas en la aplicación.            |