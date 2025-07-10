# QMS Changelog

_This project was previously called SAC._

## 2025-07-10

- Access to the server hosting the system has been established.
- All essential files from the original SAC system have been downloaded and are now stored in the SISTEMA DE CALIDAD folder.

## 2025-07-09

- Expanded and detailed functional and non-functional requirements in Docs/Requirements/Requirements.md, including manufacturing-specific modules, audit management, and Windows Server 2019 compatibility.
- Created Docs/Diagrams/ folder with .drawio files and Markdown templates for use case, class, process flow, and architecture diagrams.
- Added detailed diagram documentation in Docs/Diagrams/README.md to guide modeling and documentation for QMS/SAC.
- System now explicitly supports internal and external audits, with modules and requirements for evidence export and secure access for auditors/clients.

## 2025-07-09 (EN/ES README split)

- The main README.md is now in English only.
- Created LEEME.md as the official Spanish translation of README.md.
- All future updates to project introduction and instructions will be maintained in both files.

## 2025-07-04

- Global project name change from "SAC" to "QMS" (Quality Management System).
- Updated all documentation, code comments, scripts, and user messages to reflect the new name QMS, clarifying in each file that the project was formerly called SAC.
- Updated stakeholders in Docs/Stakeholders.md to reflect current roles and clarify the name transition.
- Documented and clarified key questions and answers from the kickoff meeting in Docs/MeetingNotes/PreguntasKickoff.txt.
- Added clarifications in all main documentation and code files about the name change and the historical context of the project.
- Maintained traceability and migration context for future audits and references.
- Created the Code/ folder with subfolders backend-node, backend-python, and frontend, clearly separating system components.
- Implemented a modern frontend in Code/frontend/ using React (.tsx), TypeScript, and Vite, with advanced TypeScript and ESLint configuration.
- Added a Node.js backend (Code/backend-node/) with modular structure, unit tests, and ES module usage.
- Added a Python backend (Code/backend-python/) with modular structure, unit tests, and requirements.txt.
- Added multiple documents and templates in Docs/ (Backlog, DefinitionOfDone, ProjectPlan, Schedule, Setup, Stakeholders, ISO9001 Manual, meeting notes, requirements, etc.).
- Added utility scripts in scripts/ (script_utils.sh).
- Standardized .gitattributes and .gitignore configuration for Node, Python, and frontend.
- Added initial unit tests in all main modules.
- Created specific README files for each submodule (frontend, backend-node, backend-python) with instructions and recommendations.
- Added issue and pull request templates in .github/.
- Documented the integration of new folders and technologies in the overall project structure.

## 2025-07-03

- Created the initial project structure.
- Added README.md, base files, and main folders.
- Initial documentation and requirements.
- Added the agenda and details of the kickoff to NotasKickoff.md.
- Added the basic files: LICENSE (MIT), CODE_OF_CONDUCT.md, SECURITY.md, CONTRIBUTING.md, and NOTICE to the project root.
- Added issue and pull request templates in `.github/ISSUE_TEMPLATE.md` and `.github/PULL_REQUEST_TEMPLATE.md`.
- Created base files for the application and scripts: `src/intranet_app/app.py`, `src/legacy_html/index.html`, `src/migration_scripts/main.py`, `scripts/script_utils.sh`, and the initial test `tests/test_app.py`.
- Added the `.gitattributes` file for text normalization.
