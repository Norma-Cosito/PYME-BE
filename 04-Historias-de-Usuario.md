HISTORIAS DE USUARIO
1. AUTENTICACIÓN Y SEGURIDAD
HU-01: Inicio de sesión seguro
Como usuario del sistema (analista o funcionario)
Quiero iniciar sesión con credenciales seguras
Para acceder únicamente a las funcionalidades autorizadas según mi rol
Criterios de aceptación:
•	Validar usuario y contraseña correctamente
•	Bloquear acceso tras 3 intentos fallidos
•	Redirigir al dashboard según rol
HU-02: Gestión de roles y permisos (RBAC)
Como administrador
Quiero asignar roles y permisos a los usuarios
Para controlar el acceso a las funcionalidades del sistema
Criterios de aceptación:
•	Crear, editar y eliminar roles
•	Asignar permisos sin afectar otros usuarios
•	Aplicar restricciones por módulo
2. GESTIÓN DEL PROCESO CREDITICIO
HU-03: Registro único de datos
Como analista de crédito
Quiero registrar los datos del cliente una sola vez
Para evitar duplicidad de información en múltiples formularios
Criterios de aceptación:
•	Datos reutilizables en diferentes módulos
•	Validación de campos obligatorios
•	Persistencia de información
HU-04: Gestión de formularios crediticios
Como analista de crédito
Quiero crear y consultar formularios del proceso crediticio
Para gestionar la información de manera digital
Criterios de aceptación:
•	Crear formularios sin errores
•	Editar y consultar información
•	Guardado automático
HU-05: Checklists inteligentes
Como analista de crédito
Quiero contar con checklists automáticos
Para asegurar que toda la documentación requerida esté completa
Criterios de aceptación:
•	Bloquear avance si falta documentación
•	Mostrar alertas de documentos faltantes
•	Validar requisitos obligatorios
3. EVALUACIÓN FINANCIERA Y PRODUCTIVA
HU-06: Evaluación financiera automatizada
Como analista de crédito
Quiero generar automáticamente estados financieros
Para agilizar el análisis del cliente
Criterios de aceptación:
•	Cálculo de balances, flujos e índices
•	Resultados precisos
•	Exportación de datos
HU-07: Evaluación productiva sectorial
Como analista
Quiero evaluar proyectos agrícolas o pecuarios
Para analizar la capacidad productiva del cliente
Criterios de aceptación:
•	Simulación de escenarios
•	Análisis sectorial correcto
•	Generación de reportes
HU-08: Scoring crediticio automático
Como sistema
Quiero calcular automáticamente el puntaje de riesgo
Para apoyar la toma de decisiones crediticias
Criterios de aceptación:
•	Evaluación basada en variables sectoriales
•	Generación automática de puntaje
•	Clasificación del riesgo
4. REPORTES Y DOCUMENTACIÓN
HU-09: Generación de reportes automáticos
Como analista
Quiero generar reportes en PDF y Excel
Para presentar resultados al comité de crédito
Criterios de aceptación:
•	Generación sin pérdida de datos
•	Descarga en múltiples formatos
•	Información estructurada
HU-10: Resumen ejecutivo automático
Como analista
Quiero obtener un resumen ejecutivo del crédito
Para facilitar la toma de decisiones
Criterios de aceptación:
•	Resumen claro y automático
•	Datos consolidados
•	Formato listo para comité
5. INTEGRACIÓN Y MONITOREO
HU-11: Integración con el CORE bancario
Como sistema
Quiero conectarme al CORE mediante API REST
Para intercambiar información financiera
Criterios de aceptación:
•	Comunicación vía JSON
•	Autenticación con JWT
•	Respuestas correctas del CORE
HU-12: Monitoreo de transacciones
Como usuario
Quiero visualizar el estado del proceso crediticio
Para hacer seguimiento en tiempo real
Criterios de aceptación:
•	Visualización de estados
•	Tiempos de proceso
•	Actualización en tiempo real
6. AUDITORÍA Y ARCHIVOS
HU-13: Registro de auditoría
Como sistema
Quiero registrar todas las acciones realizadas
Para garantizar trazabilidad
Criterios de aceptación:
•	Registro de inserciones, cambios y eliminaciones
•	Logs inalterables
•	Consulta de historial
HU-14: Gestión de documentos digitales
Como usuario
Quiero subir archivos adjuntos
Para almacenar documentación del crédito
Criterios de aceptación:
•	Almacenamiento seguro
•	Validación de archivos
•	Acceso restringido

