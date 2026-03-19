# Plataforma Virtual para la Digitalización del Proceso Crediticio - BDP S.A.M.

## 1. Descripción del Proyecto
[cite_start]Este proyecto consiste en la **Consultoría para la Provisión de Software para PYME y BE**[cite: 4]. [cite_start]El objetivo principal es desarrollar una plataforma virtual que digitalice y optimice el proceso crediticio del Banco de Desarrollo Productivo (BDP S.A.M.), integrándolo al sistema CORE bancario[cite: 4].

### Problema a Resolver
* [cite_start]Agilización de procesos manuales y eliminación de múltiples formularios físicos[cite: 4].
* [cite_start]Reducción de tiempos prolongados de análisis y carga operativa[cite: 4].
* [cite_start]Integración de scoring crediticio y monitoreo de transacciones bajo normas de seguridad[cite: 4].

---

## 2. Matriz de Stakeholders (Interesados)
| Rol | Nombre/Cargo | Influencia | Expectativa Principal |
| :--- | :--- | :--- | :--- |
| **Cliente / Patrocinador** | Alta Gerencia del BDP S.A.M. | Alto | [cite_start]Implementación en plazo, presupuesto y mejora de eficiencia[cite: 6]. |
| **Usuario Final** | Analistas de crédito y Funcionarios | Medio | [cite_start]Plataforma intuitiva que elimine hojas de cálculo externas[cite: 6]. |
| **Equipo Técnico** | Miguel Angel Chura (Gestor) y Equipo Dev | Alto | [cite_start]Requerimientos claros y entrega de software de alta calidad[cite: 6]. |

[cite_start]**Equipo de Desarrollo:** Norma Mendoza, Nicole Arratia, Roger Huarachi, Kevin Rocha, Beymar Castillo[cite: 6].

---

## 3. Especificaciones Técnicas

### Requerimientos Funcionales Clave (Top 5)
1. [cite_start]**RF-01:** Validación de credenciales y roles (Login seguro)[cite: 34].
2. [cite_start]**RF-03/05:** Evaluación financiera y generación automática de flujos/balances[cite: 34].
3. [cite_start]**RF-04:** Evaluación productiva sectorial (Agrícola/Pecuario)[cite: 34].
4. [cite_start]**RF-06:** Integración vía API REST con el CORE bancario (JSON, JWT)[cite: 34].
5. [cite_start]**RF-08:** Registro de logs de auditoría inalterables[cite: 34].

### Atributos de Calidad (No Funcionales)
* [cite_start]**Offline-First:** Operación continua en campo sin conexión mediante PWA/IndexedDB[cite: 36].
* [cite_start]**Escalabilidad:** Arquitectura modular en PostgreSQL para soportar +500 usuarios concurrentes[cite: 36].
* [cite_start]**Seguridad:** Cifrado bcrypt/Argon2 y protección WORM para logs[cite: 36].

---

## 4. Plan de Implementación y Cronograma
[cite_start]El proyecto tiene una duración total de **260 días hábiles** [cite: 48] y un presupuesto de **Bs. [cite_start]500.000,00**[cite: 51].

| Fase | Hito | Plazo |
| :--- | :--- | :--- |
| **Fase 1** | [cite_start]Análisis, diseño y maquetado de formularios[cite: 45]. | [cite_start]Hasta 40 días[cite: 45]. |
| **Fase 2** | [cite_start]Desarrollo de módulos principales e integración API[cite: 46]. | [cite_start]Hasta 140 días[cite: 46]. |
| **Fase 3** | [cite_start]Pruebas en ambiente SandBox y capacitación[cite: 47]. | [cite_start]Hasta 240 días[cite: 47]. |
| **Fase 4** | [cite_start]Paso a producción e informe final[cite: 48]. | [cite_start]Hasta 260 días[cite: 48]. |

---

## 5. Propiedad y Confidencialidad
* **Propiedad Intelectual:** Todo el código fuente es propiedad absoluta del BDP S.A.M.[cite: 42].
* [cite_start]**Confidencialidad:** Información protegida bajo acuerdos de no divulgación (NDA)[cite: 43].
