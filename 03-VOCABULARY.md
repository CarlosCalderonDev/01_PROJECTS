# 03-VOCABULARY 📚

> Documento de referencia para estandarizar términos, conceptos y vocabulario utilizado en el proyecto.

> 1. Objetivo: Definir de forma clara, breve y estandarizada cada término utilizado en el proyecto, con el fin de evitar confusiones en el equipo y acelerar la comunicación durante análisis, reuniones y desarrollo.

> 2. Convenciones x Palabra: {Tipo , Definición , Contexto de uso , Ejemplo , Relacionado con}

# 03.1-VOCABULARY-BUSINESS_LOGIC

Citas:
    Agendar
    Cancelar
    Reprogramar
    Recordatorio



Actores
Usuario
Servicio
Recurso
Notificación

# 03.2-VOCABULARY-GENERAL_SYSTEMS_THEORY_(GST)

# 03.3-VOCABULARY-PROGRAMMING

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


# 03.4-VOCABULARY-ONE_FOR_ALL

#### 🔹 Nivel 1: Conceptos básicos



---

## 📚 3. Glosario

> Agrega cada término usando esta estructura:

### **{Nombre del Término}**
- **Tipo:** (Ejemplo: Proceso, Entidad, Recurso, Estado, Actor, Regla de negocio, Métrica, etc.)
- **Definición:** Descripción corta, clara y sin ambigüedades.
- **Contexto de uso:** Dónde y cuándo aplica en el negocio/proyecto.
- **Ejemplo:** (Opcional)
- **Relacionado con:** (Opcional: lista de términos del mismo glosario)

---


### **Recurso**
- **Tipo:** Entidad del negocio
- **Definición:** Elemento que presta la atención o sobre el cual se agenda una cita. Puede ser una persona o un recurso físico.
- **Relacionado con:** *Agenda, Tipos de Recurso*

---

## 📌 4. Notas del Documento
- Este glosario es *vivo*: se actualiza conforme evoluciona el negocio o el sistema.
- Cada nuevo término debe incorporarse **antes** de nuevas reuniones o desarrollos.

