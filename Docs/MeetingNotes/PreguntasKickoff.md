# Preguntas y Respuestas - Junta de Requisitos y Kick Off QMS

_Anteriormente conocido como SAC._

**Fecha:** 4 de julio de 2025

---

## 1. Objetivo y alcance del proyecto

**Respuesta:**
Sistema de control de documentos QMS o SAC, cuyo objetivo es centralizar y gestionar de manera eficiente los documentos del Sistema de Gestión de Calidad (QMS) o Sistema de Aseguramiento de Calidad (SAC). El sistema debe permitir la creación, revisión, aprobación, distribución y archivo de documentos, asegurando el cumplimiento normativo y la trazabilidad de los cambios.

## 2. Funcionalidades mínimas requeridas

**Respuesta:**
Sistema de control de usuarios, documentos, revisiones, aprobaciones, distribución y archivo de documentos. Debe permitir la búsqueda avanzada, la gestión de versiones y el seguimiento de cambios.

## 3. Procesos/documentos prioritarios para migrar

**Respuesta:**
Identificar las funcionalidades básicas del muestreo de los archivos existentes y priorizar aquellos que son críticos para el funcionamiento del QMS/SAC. Esto incluye documentos de políticas, procedimientos, registros de auditoría y otros documentos clave.

## 4. Requisitos funcionales clave

**Respuesta:**

- Control de documentos: visualización, descarga y consulta.
- Gestión de versiones y seguimiento de cambios.
- Interfaz intuitiva y amigable.
- Creación, revisión, aprobación y distribución de documentos.
- Archivo de versiones anteriores para trazabilidad.
- Creación, revisión y aprobación de usuarios para control de acceso.

## 5. Requisitos no funcionales (seguridad, rendimiento, compatibilidad, etc.)

**Respuesta:**

- Seguridad y protección de datos.
- Acceso controlado y fácil para usuarios autorizados.
- Compatibilidad con sistemas existentes.
- Rendimiento adecuado para grandes volúmenes de documentos.
- Distribución por intranet o red local.
- Facilidad de actualización y mejora.
- Manual de usuario y documentación técnica.

## 6. Estándares o normativas a cumplir (ej. ISO9001:2015)

**Respuesta:**
El sistema debe cumplir con las normativas, asegurando que todos los procesos de gestión documental estén alineados con los requisitos de calidad establecidos por la norma ISO9001:2015. Esto incluye trazabilidad, gestión de cambios y auditoría de procesos.

## 7. Usuarios finales y roles

**Respuesta:**

- **Nivel 1:** Usuario solo lectura (descarga/visualización, sin edición).
- **Nivel 2:** Usuario con permisos de lectura, escritura y edición.
- **Nivel 3:** Usuario aprobador (revisión y aprobación, jefe directo de nivel 2).
- **Nivel 4:** Administrador de documentos (creación, edición, aprobación, eliminación, gestión de versiones y auditoría).
- **Nivel 5:** Administrador del sistema (gestión de usuarios, configuración, auditorías de seguridad, acceso completo).

## 8. Permisos o niveles de acceso requeridos

**Respuesta:**

- Asignación de permisos específicos por nivel de usuario.
- Acceso a versiones anteriores de documentos.
- Confiabilidad e integridad de los documentos.
- Visualización restringida para archivos no públicos.
- Control de acceso mediante creación, revisión y aprobación de usuarios.

## 9. Integraciones con otros sistemas

**Respuesta:**
No definido en este momento, pero se considerará la posibilidad de integraciones futuras con sistemas existentes, herramientas de gestión documental o la creación de API propias.

## 10. Dependencias técnicas o de negocio

**Respuesta:**

- Identificar dependencias con otros sistemas y procesos de negocio.
- Compatibilidad con infraestructura existente.
- Integración futura si es necesario.

## 11. Fechas clave y entregables esperados

**Respuesta:**

- Fechas clave y entregables se definirán en cada fase del proyecto.
- Considerar integraciones futuras y herramientas de gestión documental.

## 12. Criterios de éxito del proyecto

**Respuesta:**

- Métricas claras: satisfacción del usuario, cumplimiento de plazos, calidad de documentación.
- Conformidad con requisitos funcionales y no funcionales.
- Seguridad e integridad de datos.
- Capacidad para manejar grandes volúmenes de documentos.
- Cumplimiento de expectativas del departamento QMS/QA.
- Generación de informes y métricas de desempeño.

## 13. Riesgos identificados

**Respuesta:**

- Riesgos técnicos, de recursos y de tiempo.
- Considerar integraciones futuras y herramientas de gestión documental.

## 14. Limitaciones técnicas, de recursos o de tiempo

**Respuesta:**

- Identificar limitaciones de presupuesto, recursos humanos y tecnológicos.

## 15. Canal principal de comunicación

**Respuesta:**

- Slack Channel: `#qms-project`

## 16. Frecuencia de reuniones de seguimiento

**Respuesta:**

- Por definir.

## 17. Proceso para cambios de requerimientos

**Respuesta:**

- Cambios revisados posteriormente con el equipo de desarrollo.
- Documentar y aprobar cualquier cambio antes de su implementación.

## 18. Próximos pasos y responsables

**Respuesta:**

- Asignar responsabilidades específicas a cada miembro del equipo para asegurar el avance y cumplimiento de plazos.

---

### Notas adicionales

- Se hará un análisis del sistema SAC actual para identificar funcionalidades y procesos a replicar o mejorar.
- Revisión de documentos actuales y necesidades de usuarios.
- Evaluación de herramientas y tecnologías disponibles.
- Requiere acceso al servidor actual de SAC y al repositorio en GitHub para gestión de versiones y control de cambios.
