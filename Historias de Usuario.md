# Documento de Especificación: Historias de Usuario

Este documento detalla los requerimientos del sistema organizados por **Épicas**, describiendo las **Historias de Usuario**, su nivel de prioridad según la técnica **MoSCoW** y los **Criterios de Aceptación (Definición de Hecho)** para cada una.

## Épica: Seguridad y Acceso (EP01)

### HU-01: Control de Acceso y Roles
- **Historia de Usuario:** Como usuario, quiero un login seguro con roles para acceder solo a mis funciones.
- **Prioridad (MoSCoW):** Must
- **Criterio de Aceptación:** Validación de credenciales, bloqueo tras 3 intentos y JWT implementado.

### HU-02: Trazabilidad y Auditoría
- **Historia de Usuario:** Como auditor, quiero un log inalterable de cada acción para cumplir con la normativa.
- **Prioridad (MoSCoW):** Must
- **Criterio de Aceptación:** Registro automático de ID, fecha y acción en DB (protección WORM).

## Épica: Gestión de Solicitudes (EP02)

### HU-03: Digitalización de Documentos
- **Historia de Usuario:** Como analista, quiero cargar documentos digitales para eliminar el uso de papel.
- **Prioridad (MoSCoW):** Must
- **Criterio de Aceptación:** Almacenamiento seguro y visualización fluida de adjuntos.

### HU-04: Validación Documental
- **Historia de Usuario:** Como analista, quiero un checklist inteligente para saber si la documentación está completa.
- **Prioridad (MoSCoW):** Must
- **Criterio de Aceptación:** Bloqueo de avance de etapa si faltan archivos obligatorios.

## Épica: Evaluación Técnica (EP03)

### HU-05: Proyección Ganadera
- **Historia de Usuario:** Como analista agropecuario, quiero proyectar el ciclo de vida del hato ganadero.
- **Prioridad (MoSCoW):** Must
- **Criterio de Aceptación:** Cálculos automáticos de nacimientos, recría y engorde según parámetros.

### HU-06: Simulación de Escenarios Agrícolas
- **Historia de Usuario:** Como analista agrícola, quiero simular escenarios (precios/clima) mediante "Supuestos".
- **Prioridad (MoSCoW):** Should
- **Criterio de Aceptación:** Motor de reglas parametrizable sin cambiar código fuente.

## Épica: Integraciones Inteligentes (EP04)

### HU-07: Scoring Crediticio
- **Historia de Usuario:** Como sistema, quiero conectarme a la API de la Fintech aliada para obtener el scoring crediticio.
- **Prioridad (MoSCoW):** Must
- **Criterio de Aceptación:** Consumo exitoso de la API externa y visualización del puntaje en la ficha del cliente.

### HU-08: Sincronización con CORE Bancario
- **Historia de Usuario:** Como sistema, quiero sincronizar datos con el CORE bancario vía API REST.
- **Prioridad (MoSCoW):** Must
- **Criterio de Aceptación:** Intercambio de JSON validado y sin pérdida de integridad de datos.

## Épica: Movilidad - Offline (EP05)

### HU-09: Trabajo de Campo sin Conexión
- **Historia de Usuario:** Como analista de campo, quiero registrar datos sin internet para sincronizarlos después.
- **Prioridad (MoSCoW):** Must
- **Criterio de Aceptación:** Uso de PWA/IndexedDB para persistencia local y sincronización automática.

## Épica: Salidas y Reportes (EP06)

### HU-10: Generación de Resumen Ejecutivo
- **Historia de Usuario:** Como jefe de comité, quiero generar un "Resumen Ejecutivo" automático en PDF/Excel.
- **Prioridad (MoSCoW):** Must
- **Criterio de Aceptación:** Reporte fiel a los datos ingresados, exportable con un solo clic.

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

