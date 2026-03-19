# Plataforma Virtual para la Digitalización del Proceso Crediticio - BDP S.A.M.

## 1. Cuadro Resumen del Proyecto (Matriz de Control)

Este cuadro consolida los aspectos más importantes de la planificación, los responsables y los objetivos estratégicos del software.

| Categoría | Detalle Clave | Observaciones / Metas |
| :--- | :--- | :--- |
| **Nombre del Proyecto** | Consultoría para la Provisión de Software para PYME y BE | Digitalización integral del proceso crediticio. |
| **Presupuesto Total** | **Bs. 500.000,00** | Pago dividido en 4 hitos (20%, 35%, 25%, 20%). |
| **Plazo Total** | **260 días hábiles**  | Desde el análisis hasta el "Go-live" en producción. |
| **Tecnología Clave** | API REST, PostgreSQL, PWA | Integración al CORE bancario y funcionamiento offline. |
| **Propiedad** | BDP S.A.M. | El código fuente es propiedad absoluta del banco. |

## 2. Matriz de Stakeholders (Interesados)

A continuación, se detallan los actores clave que participan en el proyecto y sus expectativas principales.

| Rol | Nombre / Cargo | Influencia | Expectativa Principal |
| :--- | :--- | :--- | :--- |
| **Cliente / Patrocinador** | Alta Gerencia del BDP S.A.M. | **Alto** | Implementación en plazo, presupuesto y mejora de eficiencia. |
| **Usuario Final** | Analistas de crédito y Funcionarios | **Medio** | Plataforma fácil de usar que elimine procesos manuales. |
| **Equipo Técnico** | Norma Mendoza (Gestor) + Equipo Dev | **Alto** | Requerimientos claros y entrega de software de alta calidad. |

## 3. Resumen de Ejecución (Hitos y Entregables)

El cronograma se divide en cuatro grandes fases de trabajo para asegurar una implementación controlada.

| Fase | Descripción de Actividades | Plazo (Días Hábiles) |
| :--- | :--- | :--- |
| **Fase 1: Análisis** | Maquetado de formularios y definición de transiciones. | Hasta 40 días. |
| **Fase 2: Desarrollo** | Construcción de módulos y conexión API al CORE. | Hasta 140 días. |
| **Fase 3: Pruebas** | Uso de **SandBox**, validación de calculadoras y capacitación. | Hasta 240 días. |
| **Fase 4: Producción** | Paso a producción (Go-live) y transferencia tecnológica. | Hasta 260 días. |

## 4. Requerimientos Destacados

### Funcionales (RF)
* **Integración:** Comunicación vía API REST con el CORE bancario.
* **Automatización:** Generación automática de flujos, balances e índices financieros.
* **Sectorial:** Evaluación especializada para sectores agrícolas y pecuarios.

### No Funcionales (RNF)
* **Offline-First:** Operación continua en campo sin conexión a internet.
* **Seguridad:** Registro de logs de auditoría inalterables (protección WORM).
* **Escalabilidad:** Soporte para un mínimo de 500 usuarios concurrentes.

## 5. Confidencialidad y Propiedad
Toda la información técnica y de negocio contenida en este repositorio es estrictamente confidencial. El código fuente desarrollado es propiedad exclusiva del **BDP S.A.M.**
