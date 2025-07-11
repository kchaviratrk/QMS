# Contexto y funcionalidades del sistema QMS/SAC

Fecha actual: 10 de julio de 2025
Sistema operativo: macOS

## Estructura actual del workspace

```
changelog.md
CODE_OF_CONDUCT.md
context_sac.md
CONTRIBUTING.md
LEEME.md
LICENSE
NOTICE
README.md
ROADMAP.md
SECURITY.md
Code/
	backend-node/
	backend-python/
	frontend/
Docs/
	Backlog.md
	DefinitionOfDone.md
	ProjectPlan.md
	Schedule.md
	Setup.md
	Stakeholders.md
	Diagrams/
	ISO9001/
	MeetingNotes/
	Requirements/
scripts/
	script_utils.sh
SISTEMA DE CALIDAD/
	[INDICE DE DOCUMENTOS DE CONSULTA.htm
	~$dice de Alertas de Calidad..htm
	adapterplatinumgreen - Ivenn Duran.SLDPRT
	Auditorias 2024.htm
	BUSCAS AUDITORIAS DE ANOS ATRAS.htm
	CATALOGO DE TAPES.htm
	CONSULTAR EN “ESTACION DE CONSULTA”.htm
	GREEN TAPE.htm
	INDICE CAPAS INTERNAS Y EXTERNAS 2024.htm
	INDICE CAPAS INTERNAS Y EXTERNAS.htm
	Indice CRITERIOS DE ACEPTACION CALIDAD.htm
	Indice de Alertas de Calidad..htm
	Indice de Auditorias Internas del 2022.htm
	INDICE DE CAPAS EXTERNAS 2022.htm
	INDICE DE CAPAS EXTERNAS 2024.htm
	INDICE DE CAPAS EXTERNAS.htm
	INDICE DE CAPAS INTERNAS 2024.htm
	INDICE DE CAPAS INTERNAS.htm
	INDICE DE CAPAS.htm
	INDICE DE DOCUMENTOS EXTERNOS.htm
	ÍNDICE DE FAIs.htm
	Indice de Formatos  de  CALIBRACION.htm
	Indice de Formatos  de  Calidad.htm
	Indice de Formatos  de  Compras.htm
	Indice de Formatos  de  EHS.htm
	Indice de Formatos  de  Embarques.htm
	Indice de Formatos  de  INGENIERIA.htm
	Indice de Formatos  de  IT.htm
	Indice de Formatos  de  MANTENIMIENTO.htm
	Indice de Formatos  de  Planeacion.htm
	Indice de Formatos  de  PRODUCCION.htm
	Indice de Formatos  de  Sistemas de Calidad.htm
	Indice de Formatos  de almacen.htm
	Indice de Formatos  de Recursos Humanos.htm
	Indice de Formatos entrenamiento.htm
	Indice de Formatos.htm
	Indice de Instruccion IT.htm
	INDICE DE INSTRUCCIONES  LIME TAPE.htm
	INDICE DE INSTRUCCIONES DE ALMACEN.htm
	Indice de Instrucciones de AYUDAS VISUALES..htm
	Indice de Instrucciones de AYUDAS VISUALES.htm
	INDICE DE INSTRUCCIONES DE BATTERY PANEL.htm
	INDICE DE INSTRUCCIONES DE BLACK TAPE 1A4.htm
	INDICE DE INSTRUCCIONES DE C1D2 E-SEAL.htm
	...
src/
	...
tests/
```

## Observaciones sobre el folder SISTEMA DE CALIDAD

- Contiene archivos estáticos (HTML, XML, etc.) de consulta, formatos, instrucciones y procedimientos.
- No tiene integración dinámica de usuarios, permisos, ni gestión centralizada de archivos.
- La gestión documental es manual y basada en archivos generados por herramientas de ofimática.
- No hay backend, base de datos ni autenticación de usuarios.
- Es necesario migrar y modernizar para lograr integración con usuarios, permisos y gestión avanzada de documentos.

## Recomendación

Para lograr un sistema moderno y funcional, se debe migrar a una arquitectura con frontend (React + TypeScript), backend (Node.js + Express), base de datos y gestión de usuarios, roles y permisos, como se describe en el contexto general de QMS/SAC.

Este archivo resume el estado actual y la estructura del workspace para referencia en el desarrollo y migración del sistema.

## Funcionalidades principales

- Gestión documental: creación, edición, revisión, aprobación, distribución y archivo de documentos.
- Control de versiones y trazabilidad de cambios.
- Búsqueda avanzada y eficiente de documentos.
- Gestión de usuarios y roles (lectura, edición, aprobación, administración, auditoría).
- Permisos granulares y control de acceso por nivel de usuario.
- Auditoría de procesos y registro de acciones (para auditorías internas/externas).
- Exportación de evidencia y reportes en PDF/Excel.
- Migración y consulta de documentos históricos (HTML legado).
- Interfaz moderna, intuitiva y segura.
- Integración futura con otros sistemas y APIs.
- Soporte para restauración ante fallos y respaldo automático.
- Compatibilidad con Windows Server 2019 y navegadores modernos.

## Roles de usuario

- Nivel 1: Solo lectura
- Nivel 2: Edición
- Nivel 3: Aprobador
- Nivel 4: Administrador documental
- Nivel 5: Administrador del sistema

## Requisitos no funcionales

- Seguridad y protección de datos
- Rendimiento para grandes volúmenes
- Facilidad de mantenimiento y escalabilidad
- Acceso por intranet/red local
- Cumplimiento de normativas y trazabilidad

## Arquitectura sugerida

- Frontend: React + TypeScript + Vite
- Backend: Node.js + Express
- Base de datos: SQL Server, PostgreSQL, etc.
- Almacenamiento de documentos
- Integración con sistemas internos y externos

## Documentación y diagramas

- Diagramas de casos de uso, clases, procesos y arquitectura en Docs/Diagrams/
- Requerimientos funcionales y no funcionales en Docs/Requirements/
- Roadmap, backlog y plan de proyecto en Docs/

Este contexto sirve como base para el desarrollo, migración y mejora del sistema QMS/SAC. Para detalles técnicos y ejemplos, consulta los archivos en Docs/ y la estructura del repositorio.

# Resumen de migración y desarrollo QMS/SAC

## Estado actual (SAC en SISTEMA DE CALIDAD)

- El sistema SAC está compuesto por archivos estáticos (HTML, XML, Word, Excel, etc.) organizados por departamentos y tipos de documentos.
- No existe integración de usuarios, permisos, ni backend; la gestión documental es manual y no centralizada.
- Los archivos contienen procedimientos, formatos, instrucciones y registros, pero no hay lógica de negocio ni interacción dinámica.
- No hay base de datos, autenticación, ni API; todo es consulta y edición manual.

## Objetivo del nuevo sistema (QMS en Code/)

- Migrar y mejorar las funcionalidades útiles del SAC, integrando todo en una arquitectura moderna y centralizada.
- El desarrollo se realizará en el folder Code/ usando:
  - Frontend: React + Vite + TypeScript
  - Backend: Node.js + Express
  - Base de datos relacional (ej. PostgreSQL, SQL Server)
  - Gestión de usuarios, roles y permisos
  - API REST para integración y automatización
  - Interfaz intuitiva y segura, con control de acceso y trazabilidad

## Proceso sugerido

1. Analizar y documentar las funcionalidades y procesos clave del SAC que deben migrarse/mejorarse.
2. Definir la estructura inicial del nuevo sistema en Code/ (carpetas, módulos, endpoints, modelos de datos).
3. Desarrollar el backend con Node.js/Express y el frontend con React/TypeScript, integrando la lógica de negocio y gestión documental.
4. Implementar autenticación, control de usuarios y permisos.
5. Migrar los documentos y datos relevantes del SAC al nuevo sistema.
6. Validar, probar y documentar todo el proceso.

## Recursos útiles

- [React Quick Start](https://reactjs.org/docs/getting-started.html): Componentes, JSX, manejo de estado, eventos, listas, estilos.
- [Node.js Docs](https://nodejs.org/en/docs/): Módulos, HTTP, File System, API, procesos.
- [Express Docs](https://expressjs.com/en/starter/installing.html): Instalación, rutas, middlewares, estructura de proyecto.
- [VS Code API](https://code.visualstudio.com/api): Para futuras integraciones o extensiones VS Code.

## Siguiente paso

- Definir la estructura inicial del folder Code/ y los módulos principales del nuevo QMS.
- Documentar los procesos y funcionalidades a migrar/mejorar.

Este archivo sirve como guía y referencia para la migración y desarrollo del nuevo sistema QMS, integrando lo mejor del SAC y modernizando la gestión documental y de usuarios.
