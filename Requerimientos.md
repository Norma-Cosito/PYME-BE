# Guía de Trabajo: Identificación de Requerimientos para un Proyecto Real

[cite_start]**Versión del Documento:** 1.0 [cite: 2]  
[cite_start]**Fecha:** 12/02/2026 [cite: 3]  
[cite_start]**Autores:** Miguel Angel Chura Condori, Norma Mendoza Layme, Nicole Abigail Arratia Chipana, Roger Huarachi Rojas, Kevin Jhonatan Rocha, Beymar Castillo Cordova[cite: 4, 44].

---

## 1. Introducción y Objetivo
[cite_start]El propósito de esta guía es proporcionar un marco estructurado para descubrir, analizar y documentar los requerimientos de un proyecto de software o ingeniería[cite: 5, 6]. [cite_start]Un buen levantamiento reduce riesgos de fracaso, sobrecostos y malentendidos[cite: 7].

### ¿Qué es un Requerimiento?
[cite_start]Es una condición o capacidad que debe cumplir el sistema para satisfacer un contrato, estándar o especificación formal[cite: 8, 9].

---

## [cite_start]2. Fases de la Identificación [cite: 10]

### [cite_start]Fase A: Definición del Contexto y Stakeholders [cite: 11]
* **Stakeholders Clave:** ¿Quién paga? ¿Quién lo usa? [cite_start]¿Quién lo mantiene? [cite: 13]
* [cite_start]**Problema de Negocio:** ¿Qué necesidad resuelve este software? [cite: 14]
* [cite_start]**Alcance (Scope):** Lo que incluye y lo que no incluye el proyecto[cite: 15].

### [cite_start]Fase B: Técnicas de Elicitación [cite: 16]
* [cite_start]**Entrevistas:** Reuniones 1 a 1[cite: 18].
* [cite_start]**Lluvia de Ideas:** Sesión grupal sin filtros[cite: 19].
* [cite_start]**Observación:** Ver cómo trabajan los usuarios[cite: 20].
* [cite_start]**Análisis Documental:** Revisar reportes y sistemas actuales[cite: 21].
* [cite_start]**Prototipado:** Bocetos rápidos para feedback[cite: 22].

### [cite_start]Fase C: Clasificación de Requerimientos [cite: 23]
1.  [cite_start]**Negocio:** Objetivos de alto nivel de la organización[cite: 24, 25].
2.  [cite_start]**Usuario:** Lo que el usuario necesita hacer[cite: 26, 27].
3.  [cite_start]**Funcionales (RF):** Comportamientos específicos ("El sistema debe...")[cite: 28, 29].
4.  [cite_start]**No Funcionales (RNF):** Atributos de calidad (URPS: Usabilidad, Confiabilidad, Rendimiento, Soporte)[cite: 32, 33, 34, 35, 36, 37].

---

## [cite_start]3. Hoja de Trabajo Práctica [cite: 39]

### 3.1. [cite_start]Ficha del Proyecto [cite: 41]
| Concepto | Descripción |
| :--- | :--- |
| **Nombre del Proyecto** | [cite_start]CONSULTORÍA PARA LA PROVISIÓN DE SOFTWARE PARA PYME Y BE [cite: 42] |
| **Problema a Resolver** | [cite_start]Proceso crediticio lento y manual en BDP S.A.M. que requiere agilidad, digitalización y trazabilidad[cite: 42]. |
| **Objetivo Principal** | [cite_start]Implementar una plataforma virtual integrada al CORE bancario para optimizar el proceso crediticio[cite: 42]. |

### 3.2. [cite_start]Matriz de Stakeholders [cite: 43]
| Rol | Nombre/Cargo | Influencia | Expectativa Principal |
| :--- | :--- | :--- | :--- |
| Cliente / Patrocinador | Directorio y Alta Gerencia BDP | Alto | [cite_start]Eficiencia y cumplimiento de plazos[cite: 44]. |
| Usuario Final | Analistas de crédito y funcionarios | Medio | [cite_start]Plataforma fácil de usar y ágil[cite: 44]. |
| Equipo Técnico | Miguel Chura condori (Gestor de pila), Norma Mendoza (Devs), Nicole Arratia(Devs), Roger Huarachi(Devs), Kevin Rocha(Devs), Beymar Castillo(Devs) | - | [cite_start]Desarrollo y ejecución técnica[cite: 4, 44]. |

### 3.3. [cite_start]Listado de Requerimientos Funcionales (RF) [cite: 45]
| ID | Descripción | Prioridad | Criterio de Aceptación |
| :--- | :--- | :--- | :--- |
| **RF-01** | Validar credenciales (Login) | Must | [cite_start]Bloqueo tras 3 intentos fallidos[cite: 47]. |
! **RF-01.01**|
| **RF-02** | Gestión de solicitudes de crédito | Must | [cite_start]Crear, editar y consultar sin errores[cite: 48, 49, 50]. |
| **RF-03** | Evaluaciones financieras automáticas | Must | [cite_start]Cálculos correctos y reportes exportables[cite: 53, 54, 55]. |
| **RF-03.01** | Carga de Datos y Consolidación: El sistema debe permitir ingresar el balance general y el estado de resultados (o los datos equivalentes para micro-segmentos que no llevan contabilidad formal). Queremos que, al ingresar estos datos, el sistema calcule automáticamente los ratios financieros estándar: liquidez, solvencia, rotación de inventarios, etc. | Must | [cite_start]Cálculos correctos y reportes exportables[cite: 53, 54, 55]. |
| **RF-03.02** | Capacidad de Pago: Esta es la "joya de la corona". Necesitamos que el software proyecte el flujo de caja del cliente y determine, de manera automática, cuánto puede pagar mensualmente sin asfixiar su negocio. Si el oficial cambia una variable (como el plazo del crédito), el cálculo de la capacidad de pago debería actualizarse al instante.| Must | [cite_start]Cálculos correctos y reportes exportables[cite: 53, 54, 55]. |
| **RF-03.03** | Análisis Comparativo: Nos gustaría que el sistema compare los indicadores del cliente actual con promedios del mismo sector (por ejemplo, comparar una manufacturera de muebles con el promedio de ese rubro).| Must | [cite_start]Cálculos correctos y reportes exportables[cite: 53, 54, 55]. |
| **RF-04** | Integración API REST con CORE | Must | [cite_start]Validación JWT e intercambio JSON exitoso[cite: 57, 58, 59]. |
| **RF-04.01** | Consulta de Datos del Cliente (GET): Cuando un oficial inicia una solicitud, el sistema debe "llamar" al Core mediante la API para verificar si el cliente ya existe. Necesitamos traer de vuelta sus datos básicos, su historial de créditos actuales, sus saldos en cuentas y, muy importante, su calificación de riesgo vigente en el sistema.| Must | [cite_start]Validación JWT e intercambio JSON exitoso[cite: 57, 58, 59]. |
| **RF-04.02** | Sincronización de Tablas Maestras: El software de la consultoría debe estar alimentado por las tasas de interés, plazos máximos y tipos de garantías que el Core tiene parametrizados. No queremos que un oficial de crédito use una tasa que ya caducó.| Must | [cite_start]Validación JWT e intercambio JSON exitoso[cite: 57, 58, 59]. |
| **RF-04.03** | Escritura de la Operación (POST/PUT): Una vez que el crédito es aprobado en la nueva plataforma, toda la estructura (plan de pagos, datos de la garantía, condiciones) debe "viajar" al Core para su desembolso. No queremos que nadie tenga que transcribir datos manualmente del software nuevo al Core antiguo. Eso es fuente de errores. | Must | [cite_start]Validación JWT e intercambio JSON exitoso[cite: 57, 58, 59]. |
| **RF-05** | Reportes automáticos (PDF/Excel) | Must | [cite_start]Generación sin pérdida de información[cite: 60, 61, 62, 63]. |
| **RF-05.01** | Informe de Propuesta de Crédito (PDF): Este es un documento formal, con el logo del BDP, que resume toda la evaluación. Debe incluir:
Datos generales del cliente y su unidad productiva.
Cuadros de estados financieros comparativos.
El análisis de los ratios que mencionamos antes.
La conclusión del oficial de crédito.
Nota importante: Este PDF debe ser "no editable" para garantizar la integridad de la información que llega al comité.| Must | [cite_start]Generación sin pérdida de información[cite: 60, 61, 62, 63]. |
| **RF-05.02** | Plan de Pagos Proyectado (PDF/Excel): Un documento que el oficial pueda entregarle al cliente ahí mismo, en su negocio, para que vea cómo quedarían sus cuotas.qa| Must | [cite_start]Generación sin pérdida de información[cite: 60, 61, 62, 63]. |
| **RF-05.03** | Generación de Reportes de Seguimiento y Mora en formato Excel: El sistema deberá permitir al Gerente generar un archivo en formato Excel que consolide información actualizada sobre el estado de las solicitudes y el desempeño de los oficiales.| Must | [cite_start]Generación sin pérdida de información[cite: 60, 61, 62, 63]. |
| **RF-06** | Logs de auditoría | Must | [cite_start]Registro de usuario, fecha y acción[cite: 64, 65, 66, 67]. |
| **RF-06.01** | | Trazabilidad de Decisiones de Crédito: El sistema permitirá verificar de manera transparente y auditable todo el proceso de aprobación de un crédito (por ejemplo, uno de 100.000 bolivianos), asegurando control interno y cumplimiento normativo.| [cite_start]Registro de usuario, fecha y acción[cite: 64, 65, 66, 67]. |
| **RF-06.02** | Control y Registro de Modificaciones de Datos Sensibles: El sistema garantizará que toda modificación de información crítica deje evidencia auditable, evitando alteraciones sin registro y fortaleciendo el control interno.| Must | [cite_start]Registro de usuario, fecha y acción[cite: 64, 65, 66, 67]. |
| **RF-06.03** | Registro de Intentos de Acceso y Eventos de Seguridad: El sistema garantizará el control y la trazabilidad de accesos indebidos o intentos fallidos, reduciendo riesgos de fraude, accesos no autorizados y vulneraciones de información.| Must | [cite_start]Registro de usuario, fecha y acción[cite: 64, 65, 66, 67]. |
| **RF-07** | Administración de roles y perfiles | Must | [cite_start]Gestión de permisos sin afectar otros usuarios[cite: 68, 69, 70, 71]. |
| **RF-08** | Almacenamiento seguro de archivos | Must | [cite_start]Directorios protegidos y autorizados[cite: 72, 73, 74, 75]. |
| **RF-09** | Scoring crediticio y análisis de riesgo | Should | [cite_start]Puntuación automática según criterios[cite: 76, 77, 78, 79]. |
| **RF-10** | Seguimiento de trámites en tiempo real | Should | [cite_start]Visualización del estado del trámite[cite: 80, 81, 82, 83]. |
| **RF-15** | Aplicación móvil independiente | Won't | [cite_start]Fuera del alcance en esta fase[cite: 100, 101, 102, 103]. |

### 3.4. [cite_start]Listado de Requerimientos No Funcionales (RNF) [cite: 104]
| ID | Categoría | Descripción Técnica | Métrica de Éxito |
| :--- | :--- | :--- | :--- |
| **RNF-01** | Seguridad | Hashing de contraseñas | [cite_start]Uso de bcrypt/Argon2[cite: 105]. |
| **RNF-02** | Rendimiento | Tiempo de respuesta | [cite_start]Menos de 1 seg con 10k registros[cite: 105]. |
| **RNF-03** | Compatibilidad | Web Responsive | [cite_start]Móvil y Escritorio[cite: 105]. |
| **RNF-04** | Disponibilidad | Alta disponibilidad | [cite_start]99% de uptime mensual[cite: 105]. |
| **RNF-05** | Escalabilidad | Escalamiento horizontal | [cite_start]500+ usuarios concurrentes[cite: 105]. |

---

## [cite_start]4. Validación y Cierre [cite: 108, 109]
* [cite_start][x] ¿Son los requerimientos claros y sin ambigüedades? [cite: 110]
* [cite_start][x] ¿Son los requerimientos medibles? [cite: 111]
* [cite_start][ ] ¿Todos los stakeholders han aprobado esta lista? [cite: 112]
* [cite_start][ ] ¿Se han identificado riesgos técnicos complejos? [cite: 113]

**Firma:** __________________________  
[cite_start]**Fecha:** __________________ [cite: 114, 115]


