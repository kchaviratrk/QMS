# Diagramas QMS - Plantillas y Referencias

Este directorio contiene los diagramas principales del sistema QMS/SAC. Los archivos .drawio pueden ser editados en draw.io o diagrams.net. Aquí se incluyen plantillas en Markdown para documentar cada diagrama.

---

## Use Case Diagram: Document Approval and Audit Management

**Descripción:**
Diagrama de casos de uso para la gestión de aprobación de documentos y auditorías internas/externas.

**Actores:**

- Usuario (todos los niveles)
- Administrador de documentos
- Administrador del sistema
- Auditor externo/interno

**Casos de uso principales:**

- Crear documento
- Editar documento
- Enviar a aprobación
- Aprobar/rechazar documento
- Consultar historial de auditoría
- Exportar evidencia para auditoría

---

## Class Diagram: Core Entities (User, Document, Audit, NonConformity, Equipment)

**Descripción:**
Diagrama de clases que representa las entidades principales del sistema y sus relaciones.

**Clases sugeridas:**

- Usuario
- Documento
- VersiónDocumento
- Auditoría
- NoConformidad
- EquipoMedición
- Proveedor

**Relaciones:**

- Un Documento tiene muchas VersionesDocumento
- Un Usuario puede crear, editar, aprobar Documentos
- Una Auditoría puede estar asociada a múltiples NoConformidades

---

## Process Flow: Non-Conformity Management

**Descripción:**
Flujo de proceso para la gestión de no conformidades desde su detección hasta el cierre.

**Pasos sugeridos:**

1. Detección de no conformidad
2. Registro en el sistema
3. Análisis de causa raíz
4. Definición de acción correctiva
5. Implementación y seguimiento
6. Verificación y cierre

---

## Architecture Diagram: QMS on Windows Server 2019

**Descripción:**
Diagrama de arquitectura que muestra la integración del sistema QMS en un entorno Windows Server 2019.

**Componentes sugeridos:**

- Servidor Windows 2019
- Base de datos (SQL Server, PostgreSQL, etc.)
- Backend (Node.js/Python)
- Frontend (React/Vite)
- Almacenamiento de documentos
- Usuarios internos y externos (auditores, clientes)

---

> Edita los archivos .drawio correspondientes para mantener actualizados los diagramas visuales.
