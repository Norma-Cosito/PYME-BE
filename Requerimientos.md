# Guía de Trabajo: Identificación de Requerimientos para un Proyecto Real

## 1. Información del Equipo
| Rol | Integrantes | Estado |
| :--- | :--- | :--- |
| **Equipo Técnico** | Miguel Chura Condori (Gestor de pila), Norma Mendoza (Dev), Nicole Arratia (Dev), Roger Huarachi (Dev), Kevin Rocha (Dev), Beymar Castillo (Dev) | Desarrollo y ejecución técnica |

---

## 3.3. Listado de Requerimientos Funcionales (RF)
| ID | Descripción | Prioridad | Criterio de Aceptación |
| :--- | :--- | :--- | :--- |
| **RF-01** | **Validar credenciales (Login):** Autenticación de usuarios al sistema. | Must | Bloqueo tras 3 intentos fallidos. |
| **RF-02** | **Gestión de solicitudes de crédito:** Crear, editar y consultar solicitudes. | Must | Operaciones sin errores de integridad. |
| **RF-03** | **Evaluaciones financieras automáticas:** Cálculos de ratios y salud financiera. | Must | Cálculos correctos y reportes exportables. |
| **RF-03.01** | **Carga de Datos y Consolidación:** Ingreso de balance general y estado de resultados para cálculo automático de ratios (liquidez, solvencia, etc.). | Must | Resultados validados matemáticamente. |
| **RF-03.02** | **Capacidad de Pago:** Proyección de flujo de caja y determinación de cuota mensual ajustable según variables (plazo/monto). | Must | Actualización instantánea del cálculo. |
| **RF-03.03** | **Análisis Comparativo:** Comparación de indicadores del cliente frente a promedios del sector industrial/comercial. | Must | Visualización de desviaciones estándar. |
| **RF-04** | **Integración API REST con CORE:** Conexión con el sistema central del banco. | Must | Validación JWT e intercambio JSON exitoso. |
| **RF-04.01** | **Consulta de Datos del Cliente (GET):** Verificación de existencia, historial crediticio y calificación de riesgo desde el Core. | Must | Tiempo de respuesta < 2 segundos. |
| **RF-04.02** | **Sincronización de Tablas Maestras:** Actualización de tasas de interés, plazos y garantías parametrizadas en el Core. | Must | Datos actualizados al inicio de sesión. |
| **RF-04.03** | **Escritura de la Operación (POST/PUT):** Envío de estructura de crédito aprobada al Core para desembolso automático. | Must | Cero transcripción manual necesaria. |
| **RF-05** | **Reportes automáticos (PDF/Excel):** Generación de documentos de salida. | Must | Generación sin pérdida de información. |
| **RF-05.01** | **Informe de Propuesta de Crédito (PDF):** Documento formal no editable con logo BDP, cuadros comparativos y conclusiones. | Must | Formato PDF/A (no editable). |
| **RF-05.02** | **Plan de Pagos Proyectado (PDF/Excel):** Documento informativo para el cliente con el detalle de cuotas. | Must | Descarga inmediata en sitio. |
| **RF-05.03** | **Reportes de Seguimiento y Mora (Excel):** Consolidado para gerencia sobre el estado de solicitudes y desempeño de oficiales. | Must | Formato .xlsx compatible. |
| **RF-06** | **Logs de auditoría:** Registro de actividad de usuarios. | Must | Registro de usuario, fecha y acción. |
| **RF-06.01** | **Trazabilidad de Decisiones:** Historial auditable del proceso de aprobación (ej. créditos de 100k BOB). | Must | Log inalterable. |
| **RF-06.02** | **Control de Modificaciones Sensibles:** Registro de cambios en datos críticos del cliente o montos. | Must | Alerta de modificación de datos. |
| **RF-06.03** | **Registro de Eventos de Seguridad:** Log de intentos fallidos y accesos no autorizados. | Must | Reporte de seguridad diario. |
| **RF-07** | **Administración de roles y perfiles:** Control de acceso granular. | Must | Gestión de permisos centralizada. |
| **RF-08** | **Almacenamiento seguro de archivos:** Resguardo de documentos digitales. | Must | Directorios protegidos y cifrados. |
| **RF-09** | **Scoring crediticio:** Puntuación automática de riesgo. | Should | Basado en algoritmos predefinidos. |
| **RF-10** | **Seguimiento en tiempo real:** Visualización del estado del trámite para el cliente/oficial. | Should | Dashboard de estados. |
| **RF-15** | **Aplicación móvil independiente:** App nativa para dispositivos. | Won't | Fuera de alcance en esta fase. |

---

## 3.4. Listado de Requerimientos No Funcionales (RNF)
| ID | Categoría | Descripción Técnica | Métrica de Éxito |
| :--- | :--- | :--- | :--- |
| **RNF-01** | Seguridad | Hashing de contraseñas de alta seguridad. | Uso de **bcrypt** o **Argon2**. |
| **RNF-02** | Rendimiento | Optimización de consultas y procesos. | Respuesta < 1 seg con 10k registros. |
| **RNF-03** | Compatibilidad | Interfaz adaptable a dispositivos. | Diseño **Web Responsive**. |
| **RNF-04** | Disponibilidad | Continuidad del servicio. | **99.9%** de uptime mensual. |
| **RNF-05** | Escalabilidad | Capacidad de crecimiento del sistema. | Soporte para **500+** usuarios concurrentes. |

---

## 4. Validación y Cierre
- [x] ¿Son los requerimientos claros y sin ambigüedades?
- [x] ¿Son los requerimientos medibles?
- [ ] ¿Todos los stakeholders han aprobado esta lista?
- [ ] ¿Se han identificado riesgos técnicos complejos?

**Firma:** __________________________  
**Fecha:** __________________________
