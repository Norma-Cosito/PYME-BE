#Guía de Trabajo: Identificación de Requerimientos para un Proyecto Real##

Versión del Documento: 1.0
*Fecha:** [12/02/2026]
*Autores:** [Miguel Angel Chura Condori, Norma Mendoza Layme, Nicole Abigail Arratia Chipana, Roger Huarachi Rojas, Kevin Jhonatan Rocha, Beymar Castillo Cordova]

1. Introducción y Objetivo
El propósito de esta guía es proporcionar un marco estructurado para descubrir, analizar y documentar los requerimientos de un proyecto de software o ingeniería. Un buen levantamiento de requerimientos reduce el riesgo de fracaso del proyecto, sobrecostos y malentendidos con el cliente.
¿Qué es un Requerimiento?
Es una condición o capacidad que debe cumplir el sistema para satisfacer un contrato, estándar, especificación u otro documento formalmente impuesto.

2. Fases de la Identificación
Fase A: Definición del Contexto y Stakeholders (Interesados)
Antes de hablar de funciones, debemos entender quiénes interactúan con el sistema.
●Stakeholders Clave: ¿Quién paga? ¿Quién lo usa? ¿Quién lo mantiene?
●Problema de Negocio: ¿Qué dolor o necesidad resuelve este software?
●Alcance (Scope): ¿Qué INCLUYE el proyecto y qué NO INCLUYE (Exclusiones)?
Fase B: Técnicas de Elicitación (Extracción de Información)
Selecciona al menos dos técnicas para tu proyecto:
1.Entrevistas: Reuniones 1 a 1 con usuarios clave.
2.Lluvia de Ideas (Brainstorming): Sesión grupal para generar ideas sin filtros.
3.Observación (Shadowing): Ver cómo trabajan los usuarios actualmente.
4.Análisis Documental: Revisar reportes actuales, excels o sistemas legados.
5.Prototipado: Mostrar bocetos rápidos para recibir feedback.
Fase C: Clasificación de Requerimientos
1. Requerimientos de Negocio
Objetivos de alto nivel de la organización (Ej: "Reducir el tiempo de facturación en un 20%").
2. Requerimientos de Usuario
Lo que el usuario necesita hacer con el sistema (Ej: "El cajero necesita registrar una venta rápidamente").
3. Requerimientos Funcionales (RF)
Comportamientos específicos del sistema. Se redactan generalmente como:
"El sistema debe permitir [ACCIÓN] a [ACTOR] para [OBJETIVO]."
●Ejemplo: El sistema debe permitir al administrador generar un reporte PDF de ventas mensuales.
4. Requerimientos No Funcionales (RNF) - Atributos de Calidad
Cómo debe comportarse el sistema (Restricciones). Usa el acrónimo URPS:
●Usabilidad (Facilidad de uso, colores, accesibilidad).
●Reliability (Confiabilidad, disponibilidad 24/7).
●Performance (Rendimiento, tiempos de carga < 2 seg).
●Supportability (Mantenibilidad, facilidad de instalación, escalabilidad).
●Extra: Seguridad (Encriptación, roles, backups).
3. Hoja de Trabajo Práctica (Plantilla)
Instrucciones: Rellena esta sección con los datos de tu proyecto real.
3.1. Ficha del Proyecto
Concepto	Descripción
Nombre del Proyecto	CONSULTORÍA PARA LA PROVISIÓN DE SOFTWARE PARA PYME Y BE
Problema a Resolver	El Banco de Desarrollo Productivo (BDP S.A.M.) presenta un proceso crediticio para Pyme y Banca Empresa que requiere mayor agilidad, eficiencia y digitalización. Actualmente, el proceso implica múltiples formularios, evaluaciones manuales y tiempos prolongados de análisis, lo que genera demoras en la aprobación de créditos, mayor carga operativa y limitada trazabilidad de la información.
Además, se necesita integrar herramientas tecnológicas como scoring crediticio, monitoreo de transacciones y conexión con el sistema CORE bancario, garantizando seguridad, confidencialidad y cumplimiento normativo.

Objetivo Principal	Desarrollar e implementar una plataforma virtual que digitalice y optimice el proceso crediticio para Pyme y Banca Empresa del BDP S.A.M., permitiendo una gestión más ágil, segura y eficiente, integrada al sistema CORE del banco y alineada a las tendencias tecnológicas actuales.
3.2. Matriz de Stakeholders
Rol	Nombre/Cargo	Nivel de Influencia (Alto/Medio/Bajo)	Expectativa Principal
Cliente / Patrocinador	Directorio y Alta Gerencia del BDP S.A.M.	Alto	Que el proyecto se implemente en el plazo establecido, dentro del presupuesto y que mejore la eficiencia del proceso crediticio.
Usuario Final	Analistas de crédito y funcionarios de Pyme y Banca Empresa	Medio	Contar con una plataforma fácil de usar que agilice la evaluación y reduzca tiempos de procesamiento.
Equipo Técnico	Miguel Angel Chura Condori: (Gestor de Pila)
Norma Mendoza Layme: (Devs) 
Nicole Abigail Arratia
Chipana: (Devs)
Roger Huarachi Rojas:(Devs)
Kevin JhonatHan Rocha Rojas: (Devs)
Beymar Castillo Cordova: (Devs)		
3.3. Listado de Requerimientos Funcionales (RF)
Prioridad: MoSCoW (Must, Should, Could, Won't have)
ID	Descripción del Requerimiento	Prioridad	Criterio de Aceptación
RF-01	El sistema debe validar las credenciales de usuario (Login).	Must	Acceso denegado tras 3 intentos fallidos.
RF-02	


El sistema debe permitir el registro, edición y gestión de solicitudes de crédito para Pyme y Banca Empresa.
	Must	El usuario puede crear, modificar y consultar solicitudes sin errores.
RF-03	


El sistema debe generar automáticamente evaluaciones financieras (flujo de caja, balance general, índices financieros y proyecciones)
	Must	Cálculos automáticos correctos con resultados exportables en reportes.
RF-04	El sistema debe integrar una API REST para comunicarse con el CORE bancario e intercambiar información en formato JSON con autenticación JWT.	Must	Comunicación exitosa con el CORE, validación JWT y respuesta en formato JSON.
RF-05	El sistema debe generar reportes automáticos y permitir la exportación de información basada en los datos ingresados en los formularios.	Must	Reportes generados en formato PDF/Excel sin pérdida de información.
RF-06	El sistema debe registrar logs de auditoría (inserciones, modificaciones y eliminaciones).	Must	Registro completo de usuario, fecha y acción en el historial de auditoría.
RF-07	El sistema debe administrar perfiles y roles de usuario.	Must	Asignación y revocación de permisos sin afectar otros usuarios.
RF-08	El sistema debe permitir la carga y almacenamiento seguro de archivos digitales adjuntos.	Must	Archivos almacenados en directorios protegidos y accesibles solo por usuarios autorizados.
RF-09	El sistema debe implementar herramientas de scoring crediticio y análisis de riesgo.	Should	Generación de puntuación automática basada en criterios configurados.
RF-10	El sistema debe permitir seguimiento y monitoreo de transacciones crediticias.	Should	Visualización del estado del trámite en tiempo real.
RF-11	El sistema debe integrarse con plataformas externas del banco (Encuentro BDP y Ventana BDP).	Should	Intercambio de datos validado entre sistemas sin errores.
RF-12	El sistema debe permitir parametrización funcional por módulos.	Should	Cambios de parámetros reflejados sin necesidad de modificar código fuente.
RF-13	El sistema debe ofrecer diseño gráfico alineado a la imagen institucional.	Could	Interfaz validada por el área de comunicación del banco.
RF-14	El sistema podría permitir funcionalidades adicionales sugeridas por el proveedor.	Could	Funcionalidades implementadas sin afectar los requerimientos obligatorios.
RF-15	El sistema no incluirá aplicación móvil independiente en esta fase.	Won’t	No se desarrollará versión móvil fuera del alcance web establecido.
3.4. Listado de Requerimientos No Funcionales (RNF)
ID	Categoría	Descripción Técnica	Métrica de Éxito
RNF-01	Seguridad	Las contraseñas no deben guardarse en texto plano.	Uso de Hashing (bcrypt/Argon2).
RNF-02	Rendimiento	Tiempo de respuesta en búsquedas.	Menos de 1 segundo con 10k registros.
RNF-03	Compatibilidad	Dispositivos soportados.	Web Responsive (Móvil y Escritorio).
RNF-04	Disponibilidad	El sistema debe garantizar alta disponibilidad en producción.	99% de uptime mensual.
RNF-05	Escalabilidad	El sistema debe permitir escalamiento horizontal bajo demanda.	Soporte para 500+ usuarios concurrentes sin degradación.
RNF-06	CI/CD	Todo cambio en el código debe pasar por pipeline automatizado.	100% de despliegues mediante pipeline CI/CD.
RNF-07	Automatización	Las pruebas deben ejecutarse automáticamente en cada commit	≥ 80% cobertura de pruebas automatizadas.
RNF-08	Seguridad (DevSecOps)	El código debe ser escaneado automáticamente en busca de vulnerabilidades.	0 vulnerabilidades críticas en producción.
RNF-09	Auditoría	El sistema debe registrar logs de todas las transacciones.	Logs almacenados por mínimo 12 meses.
RNF-10	Observabilidad	El sistema debe exponer métricas de rendimiento y errores.	Dashboard con métricas en tiempo real.
RNF-11	Recuperación	Debe existir plan de recuperación ante fallos.	Restauración en menos de 30 minutos (RTO).
RNF-12	Backup	La base de datos debe tener respaldo automático diario.	Backups verificados diariamente.
RNF-13	Infraestructura	La infraestructura debe gestionarse como código (IaC).	100% infraestructura versionada en repositorio.
3.5. Reglas de Negocio y Restricciones
●(Ej: El presupuesto es limitado a $X, o el sistema debe usar base de datos Oracle por política de la empresa).
4. Validación y Cierre
Para dar por terminada esta fase, responde el siguiente Checklist:
●[X ] ¿Son los requerimientos claros y sin ambigüedades?
●[X ] ¿Son los requerimientos medibles (se pueden probar)?
●[ ] ¿Todos los stakeholders clave han aprobado esta lista?
●[ ] ¿Se han identificado riesgos técnicos asociados a los requerimientos complejos?
Firma de Aprobación del Cliente: __________________________
Fecha: __________________
