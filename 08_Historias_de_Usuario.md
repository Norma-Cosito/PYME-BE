# 8. Historias de Usuario

## 8.1. Historias de Usuario (Operativas - Usuario Final)

| ID | Rol | Historia de Usuario | Prioridad |
|----|-----|--------------------|----------|
| HU-01 | Analista de crédito | Como analista de crédito quiero registrar solicitudes de crédito para iniciar el proceso crediticio de forma digital | Alta |
| HU-02 | Analista de crédito | Como analista de crédito quiero ingresar estados financieros del cliente para analizar su capacidad de pago | Alta |
| HU-03 | Analista de crédito | Como analista de crédito quiero generar evaluaciones financieras automáticamente para mejorar la toma de decisiones | Alta |
| HU-04 | Analista de crédito | Como analista de crédito quiero obtener el scoring crediticio desde una API Fintech para acelerar la evaluación del cliente | Alta |
| HU-05 | Analista de crédito | Como analista de crédito quiero visualizar el resultado del scoring para tomar decisiones más informadas | Alta |
| HU-06 | Analista de crédito | Como analista de crédito quiero generar reportes en PDF y Excel para documentar la evaluación crediticia | Alta |
| HU-07 | Analista de crédito | Como analista de crédito quiero adjuntar documentos digitales para respaldar la evaluación | Media |
| HU-08 | Analista de crédito | Como analista de crédito quiero monitorear el estado del crédito en tiempo real para dar seguimiento al proceso | Media |


## 8.2. Historias de Usuario (Negocio / Gestión)

| ID | Rol | Historia de Usuario | Prioridad |
|----|-----|--------------------|----------|
| HU-09 | Jefatura PyME | Como jefe de la unidad PyME quiero visualizar un dashboard de créditos para monitorear el desempeño del proceso crediticio | Alta |
| HU-10 | Jefatura PyME | Como jefe de unidad quiero obtener reportes consolidados para la toma de decisiones estratégicas | Alta |
| HU-11 | Gerencia de Sistemas | Como gerencia de sistemas quiero asegurar la integración con el CORE bancario para garantizar la interoperabilidad del sistema | Alta |
| HU-12 | Gerencia de Sistemas | Como gerencia de sistemas quiero garantizar la seguridad del sistema para cumplir con normativas financieras | Alta |


## 8.3. Historias de Usuario Técnicas (DEV - Backend / Sistema)

| ID | Rol | Historia de Usuario | Prioridad |
|----|-----|--------------------|----------|
| HU-13 | Desarrollador Backend | Como desarrollador quiero crear APIs REST en formato JSON para facilitar la integración con el CORE bancario | Alta |
| HU-14 | Desarrollador Backend | Como desarrollador quiero manejar errores de integración con servicios externos para garantizar estabilidad del sistema | Alta |
| HU-15 | Administrador del sistema | Como administrador quiero gestionar roles y permisos (RBAC) para controlar el acceso según perfil de usuario | Alta |
| HU-16 | Desarrollador Backend | Como desarrollador quiero estructurar la base de datos en PostgreSQL para asegurar integridad y escalabilidad | Alta |


## 8.4. Historias de Usuario DevOps (Integración y Automatización)

| ID | Rol | Historia de Usuario | Prioridad |
|----|-----|--------------------|----------|
| HU-17 | Ingeniero DevOps | Como ingeniero DevOps quiero integrar el sistema con la API Fintech mediante REST y JWT para asegurar comunicación segura | Alta |
| HU-18 | Ingeniero DevOps | Como ingeniero DevOps quiero implementar autenticación segura para proteger el acceso al sistema | Alta |
| HU-19 | Ingeniero DevOps | Como ingeniero DevOps quiero configurar backups automáticos para garantizar recuperación ante fallos | Alta |
| HU-20 | Ingeniero DevOps | Como ingeniero DevOps quiero implementar logs de auditoría para garantizar trazabilidad de las operaciones | Alta |


## 8.5. Historias de Usuario de Operaciones (OPS - Producción)

| ID | Rol | Historia de Usuario | Prioridad |
|----|-----|--------------------|----------|
| HU-21 | Ingeniero de Operaciones | Como ingeniero de operaciones quiero monitorear el sistema en tiempo real para detectar fallos | Alta |
| HU-22 | Ingeniero de Operaciones | Como ingeniero de operaciones quiero configurar alertas automáticas para responder ante errores del sistema | Alta |
| HU-23 | Ingeniero de Operaciones | Como ingeniero de operaciones quiero garantizar disponibilidad 24/7 del sistema para asegurar continuidad del servicio | Alta |
| HU-24 | Ingeniero de Operaciones | Como ingeniero de operaciones quiero centralizar logs para auditoría y análisis de eventos | Alta |
| HU-25 | Ingeniero de Operaciones | Como ingeniero de operaciones quiero implementar seguridad en producción para proteger la información financiera | Alta |
| HU-26 | Ingeniero de Operaciones | Como ingeniero de operaciones quiero gestionar despliegues continuos para actualizar el sistema sin interrupciones | Media |
| HU-27 | Ingeniero de Operaciones | Como ingeniero de operaciones quiero asegurar la escalabilidad del sistema para soportar múltiples usuarios | Media |
| HU-28 | Ingeniero de Operaciones | Como ingeniero de operaciones quiero supervisar la integración con APIs externas para garantizar su funcionamiento | Alta |


## 8.6. Consideraciones

- Las historias están definidas bajo el enfoque ágil (Scrum).
- Se consideran actores reales del sistema: operativos, de negocio y técnicos.
- Se incluyen historias DEV, DevOps y OPS para cubrir todo el ciclo de vida del sistema.
- El sistema integra servicios externos como CORE bancario y Fintech.
