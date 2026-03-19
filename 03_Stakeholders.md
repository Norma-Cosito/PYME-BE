# Plataforma Virtual de Crédito Pyme y Empresa - BDP S.A.M.

## 1. Visión General
Este repositorio contiene la documentación y activos de la **Consultoría para la Provisión de Software para PYME y BE**. El proyecto digitaliza el ciclo de vida del crédito productivo, integrando herramientas avanzadas de scoring y conexión directa con el CORE bancario del Banco de Desarrollo Productivo.

### Objetivos Estratégicos
* **Agilidad Operativa:** Eliminar cuellos de botella mediante la automatización de formularios y flujos de aprobación.
* **Especialización Productiva:** Implementar calculadoras biológicas y sectoriales (agrícola/pecuaria).
* **Seguridad Bancaria:** Garantizar la trazabilidad total mediante auditoría inalterable y cifrado de grado financiero.

---

## 2. Matriz de Interesados (Stakeholders)

| Rol | Identidad / Cargo | Influencia | Expectativa Clave |
| :--- | :--- | :--- | :--- |
| **Patrocinador** | Alta Gerencia BDP S.A.M. | Alta | Retorno de inversión y eficiencia en plazos. |
| **Usuario Final** | Analistas de Crédito | Media | Reducción de carga manual y facilidad de uso. |
| **Equipo Técnico** | Gestor de Pilas & Devs | Alta | Requerimientos técnicos claros y calidad de código. |

**Cuerpo Técnico:** Miguel Angel Chura (Gestor), Norma Mendoza, Nicole Arratia, Roger Huarachi, Kevin Rocha, Beymar Castillo.

---

## 3. Arquitectura y Requerimientos

### Pilares Técnicos (Stack & RNF)
* **Arquitectura:** Modular con base de datos PostgreSQL.
* **Integración:** Comunicación segura vía API-REST (JWT, JSON, HATEOAS).
* **Disponibilidad:** Estrategia **Offline-First** para trabajo de campo sin conexión.
* **Auditoría:** Logs con protección WORM (inalterables).

### Funcionalidades Principales
1. **Validación de Roles:** Control de acceso basado en RBAC.
2. **Evaluación Productiva:** Simulación de escenarios de mercado y precios.
3. **Gestión de Garantías:** Conexión dinámica entre prendas pecuarias y capacidad de pago.
4. **Reportes Automáticos:** Generación de resúmenes de comité en PDF y Excel.

---

## 4. Cronograma de Ejecución (260 Días)

| Fase | Hito de Control | Entregable Principal |
| :--- | :--- | :--- |
| **01** | Análisis y Diseño | Maquetado de UX/UI y flujos de procesos. |
| **02** | Desarrollo e Integración | Módulos de crédito y conexión al CORE. |
| **03** | SandBox y Pruebas | Validación operativa y capacitación "Aprender Haciendo". |
| **04** | Paso a Producción | Transferencia tecnológica y cierre de proyecto. |

---

## 5. Aspectos Legales
* **Presupuesto:** Bs. 500.000,00 bajo modalidad de productos entregables.
* **Propiedad Intelectual:** El código fuente y la documentación son propiedad exclusiva del **BDP S.A.M.**.
* **Confidencialidad:** Sujeto a acuerdos de no divulgación (NDA).
