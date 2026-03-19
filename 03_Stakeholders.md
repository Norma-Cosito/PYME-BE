# Plataforma Virtual para la Digitalización del Proceso Crediticio - BDP S.A.M.

## 1. Cuadro Resumen del Proyecto (Matriz de Control)

Este cuadro consolida los aspectos más importantes de la planificación, los responsables y los objetivos estratégicos del software.

| Categoría | Detalle Clave | Observaciones / Metas |
| :--- | :--- | :--- |
| **Nombre del Proyecto** | Consultoría para la Provisión de Software para PYME y BE | Digitalización integral del proceso crediticio. |
| **Presupuesto Total** | **Bs. 500.000,00** | Pago dividido en 4 hitos (20%, 35%, 25%, 20%). |
| **Plazo Total** | [cite_start]**260 días hábiles** [cite: 48] | [cite_start]Desde el análisis hasta el "Go-live" en producción. [cite: 48] |
| **Tecnología Clave** | [cite_start]API REST, PostgreSQL, PWA [cite: 36, 38] | [cite_start]Integración al CORE bancario y funcionamiento offline. [cite: 36] |
| **Propiedad** | [cite_start]BDP S.A.M. [cite: 42] | [cite_start]El código fuente es propiedad absoluta del banco. [cite: 42] |

---

## 2. Matriz de Stakeholders (Interesados)

[cite_start]A continuación, se detallan los actores clave que participan en el proyecto y sus expectativas principales. [cite: 5, 6]

| Rol | Nombre / Cargo | Influencia | Expectativa Principal |
| :--- | :--- | :--- | :--- |
| **Cliente / Patrocinador** | [cite_start]Alta Gerencia del BDP S.A.M. [cite: 6] | [cite_start]**Alto** [cite: 6] | [cite_start]Implementación en plazo, presupuesto y mejora de eficiencia. [cite: 6] |
| **Usuario Final** | [cite_start]Analistas de crédito y Funcionarios [cite: 6] | [cite_start]**Medio** [cite: 6] | [cite_start]Plataforma fácil de usar que elimine procesos manuales. [cite: 6] |
| **Equipo Técnico** | [cite_start]Miguel A. Chura (Gestor) + Equipo Dev [cite: 6] | [cite_start]**Alto** [cite: 6] | [cite_start]Requerimientos claros y entrega de software de alta calidad. [cite: 6] |

---

## 3. Resumen de Ejecución (Hitos y Entregables)

[cite_start]El cronograma se divide en cuatro grandes fases de trabajo para asegurar una implementación controlada. [cite: 44]

| Fase | Descripción de Actividades | Plazo (Días Hábiles) |
| :--- | :--- | :--- |
| **Fase 1: Análisis** | [cite_start]Maquetado de formularios y definición de transiciones. [cite: 45] | [cite_start]Hasta 40 días. [cite: 45] |
| **Fase 2: Desarrollo** | [cite_start]Construcción de módulos y conexión API al CORE. [cite: 46] | [cite_start]Hasta 140 días. [cite: 46] |
| **Fase 3: Pruebas** | [cite_start]Uso de **SandBox**, validación de calculadoras y capacitación. [cite: 47] | [cite_start]Hasta 240 días. [cite: 47] |
| **Fase 4: Producción** | [cite_start]Paso a producción (Go-live) y transferencia tecnológica. [cite: 48] | [cite_start]Hasta 260 días. [cite: 48] |

---

## 4. Requerimientos Destacados

### Funcionales (RF)
* **Integración:** Comunicación vía API REST con el CORE bancario. [cite: 34]
* [cite_start]**Automatización:** Generación automática de flujos, balances e índices financieros. [cite: 34]
* [cite_start]**Sectorial:** Evaluación especializada para sectores agrícolas y pecuarios. [cite: 34]

### No Funcionales (RNF)
* **Offline-First:** Operación continua en campo sin conexión a internet. [cite: 36]
* [cite_start]**Seguridad:** Registro de logs de auditoría inalterables (protección WORM). [cite: 36]
* [cite_start]**Escalabilidad:** Soporte para un mínimo de 500 usuarios concurrentes. [cite: 36]

---

## 5. Confidencialidad y Propiedad
[cite_start]Toda la información técnica y de negocio contenida en este repositorio es estrictamente confidencial. [cite: 43] [cite_start]El código fuente desarrollado es propiedad exclusiva del **BDP S.A.M.** [cite: 42]
