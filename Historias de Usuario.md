# Documento de Especificación de Historias de Usuario

Este documento detalla los requerimientos del sistema organizados por **Épicas**, describiendo las **Historias de Usuario**, su nivel de prioridad según la técnica **MoSCoW** y los **Criterios de Aceptación (Definición de Hecho)**.

---

## Estructura del Documento

- **Épica**
- **Historia de Usuario**
- **Prioridad (MoSCoW)**
- **Criterio de Aceptación**

---

## Épica EP01: Seguridad y Acceso

| ID    | Historia de Usuario | Prioridad | Criterio de Aceptación |
|-------|----------------------|-----------|-------------------------|
| HU-01 | Como usuario, quiero un login seguro con roles para acceder solo a mis funciones. | Must | Validación de credenciales, bloqueo tras 3 intentos y JWT implementado. |
| HU-02 | Como auditor, quiero un log inalterable de cada acción para cumplir con la normativa. | Must | Registro automático de ID, fecha y acción en DB (protección WORM). |

---

## Épica EP02: Gestión de Solicitudes

| ID    | Historia de Usuario | Prioridad | Criterio de Aceptación |
|-------|----------------------|-----------|-------------------------|
| HU-03 | Como analista, quiero cargar documentos digitales para eliminar el uso de papel. | Must | Almacenamiento seguro y visualización fluida de adjuntos. |
| HU-04 | Como analista, quiero un checklist inteligente para saber si la documentación está completa. | Must | Bloqueo de avance de etapa si faltan archivos obligatorios. |

---

## Épica EP03: Evaluación Técnica

| ID    | Historia de Usuario | Prioridad | Criterio de Aceptación |
|-------|----------------------|-----------|-------------------------|
| HU-05 | Como analista agropecuario, quiero proyectar el ciclo de vida del hato ganadero. | Must | Cálculos automáticos de nacimientos, recría y engorde según parámetros. |
| HU-06 | Como analista agrícola, quiero simular escenarios (precios/clima) mediante "Supuestos". | Should | Motor de reglas parametrizable sin cambiar código fuente. |

---

## Épica EP04: Integraciones Inteligentes

| ID    | Historia de Usuario | Prioridad | Criterio de Aceptación |
|-------|----------------------|-----------|-------------------------|
| HU-07 | Como sistema, quiero conectarme a la API de la Fintech aliada para obtener el scoring crediticio. | Must | Consumo exitoso de la API externa y visualización del puntaje en la ficha del cliente. |
| HU-08 | Como sistema, quiero sincronizar datos con el CORE bancario vía API REST. | Must | Intercambio de JSON validado y sin pérdida de integridad de datos. |

---

## Épica EP05: Movilidad - Offline

| ID    | Historia de Usuario | Prioridad | Criterio de Aceptación |
|-------|----------------------|-----------|-------------------------|
| HU-09 | Como analista de campo, quiero registrar datos sin internet para sincronizarlos después. | Must | Uso de PWA/IndexedDB para persistencia local y sincronización automática. |

---

## Épica EP06: Salidas y Reportes

| ID    | Historia de Usuario | Prioridad | Criterio de Aceptación |
|-------|----------------------|-----------|-------------------------|
| HU-10 | Como jefe de comité, quiero generar un "Resumen Ejecutivo" automático en PDF/Excel. | Must | Reporte fiel a los datos ingresados, exportable con un solo clic. |

---

## Tabla Resumen General

| Épica | Nombre de la Épica | ID Historia | Historia de Usuario | Prioridad | Criterio de Aceptación |
|-------|---------------------|-------------|----------------------|-----------|-------------------------|
| EP01 | Seguridad y Acceso | HU-01 | Como usuario, quiero un login seguro con roles para acceder solo a mis funciones. | Must | Validación de credenciales, bloqueo tras 3 intentos y JWT implementado. |
| EP01 | Seguridad y Acceso | HU-02 | Como auditor, quiero un log inalterable de cada acción para cumplir con la normativa. | Must | Registro automático de ID, fecha y acción en DB (protección WORM). |
| EP02 | Gestión de Solicitudes | HU-03 | Como analista, quiero cargar documentos digitales para eliminar el uso de papel. | Must | Almacenamiento seguro y visualización fluida de adjuntos. |
| EP02 | Gestión de Solicitudes | HU-04 | Como analista, quiero un checklist inteligente para saber si la documentación está completa. | Must | Bloqueo de avance de etapa si faltan archivos obligatorios. |
| EP03 | Evaluación Técnica | HU-05 | Como analista agropecuario, quiero proyectar el ciclo de vida del hato ganadero. | Must | Cálculos automáticos de nacimientos, recría y engorde según parámetros. |
| EP03 | Evaluación Técnica | HU-06 | Como analista agrícola, quiero simular escenarios (precios/clima) mediante "Supuestos". | Should | Motor de reglas parametrizable sin cambiar código fuente. |
| EP04 | Integraciones Inteligentes | HU-07 | Como sistema, quiero conectarme a la API de la Fintech aliada para obtener el scoring crediticio. | Must | Consumo exitoso de la API externa y visualización del puntaje en la ficha del cliente. |
| EP04 | Integraciones Inteligentes | HU-08 | Como sistema, quiero sincronizar datos con el CORE bancario vía API REST. | Must | Intercambio de JSON validado y sin pérdida de integridad de datos. |
| EP05 | Movilidad - Offline | HU-09 | Como analista de campo, quiero registrar datos sin internet para sincronizarlos después. | Must | Uso de PWA/IndexedDB para persistencia local y sincronización automática. |
| EP06 | Salidas y Reportes | HU-10 | Como jefe de comité, quiero generar un "Resumen Ejecutivo" automático en PDF/Excel. | Must | Reporte fiel a los datos ingresados, exportable con un solo clic. |

---

## Prioridades MoSCoW

| Prioridad | Descripción |
|-----------|-------------|
| Must | Requerimiento obligatorio para el funcionamiento del sistema. |
| Should | Requerimiento importante, pero no crítico para la primera versión. |
| Could | Requerimiento deseable si existen recursos y tiempo. |
| Won't | Requerimiento descartado para esta iteración. |

---

## Observaciones

- Las historias de usuario están agrupadas por épicas funcionales.
- La prioridad ha sido asignada usando la técnica **MoSCoW**.
- Los criterios de aceptación definen cuándo una historia puede considerarse completada.
