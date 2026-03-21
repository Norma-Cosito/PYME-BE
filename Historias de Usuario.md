# 1. Historias de Usuario

## 1.1. Seguridad y Acceso (EP01)

| ID     | Concepto                | Descripción |
|--------|------------------------|-------------|
| HU-01  | **Control de Acceso y Roles** | Como usuario, quiero un login seguro con roles para acceder solo a mis funciones. |
|        | **Prioridad**           | Must |
|        | **Criterio de Aceptación** | Validación de credenciales, bloqueo tras 3 intentos y JWT implementado. |

| HU-02  | **Trazabilidad y Auditoría** | Como auditor, quiero un log inalterable de cada acción para cumplir con la normativa. |
|        | **Prioridad**           | Must |
|        | **Criterio de Aceptación** | Registro automático de ID, fecha y acción en DB (protección WORM). |

---

## 1.2. Gestión de Solicitudes (EP02)

| ID     | Concepto                | Descripción |
|--------|------------------------|-------------|
| HU-03  | **Digitalización de Documentos** | Como analista, quiero cargar documentos digitales para eliminar el uso de papel. |
|        | **Prioridad**           | Must |
|        | **Criterio de Aceptación** | Almacenamiento seguro y visualización fluida de adjuntos. |

| HU-04  | **Validación Documental** | Como analista, quiero un checklist inteligente para saber si la documentación está completa. |
|        | **Prioridad**           | Must |
|        | **Criterio de Aceptación** | Bloqueo de avance si faltan archivos obligatorios. |

---

## 1.3. Evaluación Técnica (EP03)

| ID     | Concepto                | Descripción |
|--------|------------------------|-------------|
| HU-05  | **Proyección Ganadera** | Como analista agropecuario, quiero proyectar el ciclo de vida del hato ganadero. |
|        | **Prioridad**           | Must |
|        | **Criterio de Aceptación** | Cálculos automáticos de nacimientos, recría y engorde. |

| HU-06  | **Simulación de Escenarios** | Como analista agrícola, quiero simular escenarios mediante supuestos. |
|        | **Prioridad**           | Should |
|        | **Criterio de Aceptación** | Motor de reglas parametrizable sin modificar código. |

---

## 1.4. Integraciones Inteligentes (EP04)

| ID     | Concepto                | Descripción |
|--------|------------------------|-------------|
| HU-07  | **Scoring Crediticio** | Como sistema, quiero conectarme a la API fintech para obtener el scoring crediticio. |
|        | **Prioridad**           | Must |
|        | **Criterio de Aceptación** | Consumo exitoso de API y visualización del puntaje. |

| HU-08  | **Sincronización CORE** | Como sistema, quiero sincronizar datos con el CORE bancario vía API REST. |
|        | **Prioridad**           | Must |
|        | **Criterio de Aceptación** | Intercambio JSON sin pérdida de datos. |

---

## 1.5. Movilidad - Offline (EP05)

| ID     | Concepto                | Descripción |
|--------|------------------------|-------------|
| HU-09  | **Trabajo sin Conexión** | Como analista de campo, quiero registrar datos sin internet para sincronizarlos después. |
|        | **Prioridad**           | Must |
|        | **Criterio de Aceptación** | Uso de PWA + IndexedDB y sincronización automática. |

---

## 1.6. Salidas y Reportes (EP06)

| ID     | Concepto                | Descripción |
|--------|------------------------|-------------|
| HU-10  | **Resumen Ejecutivo** | Como jefe de comité, quiero generar un resumen en PDF/Excel automáticamente. |
|        | **Prioridad**           | Must |
|        | **Criterio de Aceptación** | Exportación en un clic y datos consistentes. |
