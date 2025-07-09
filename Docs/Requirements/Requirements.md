# Quality Management System (QMS/SAC) Requirements

## Objective

Centralize and efficiently manage the documents of the Quality Management System (QMS) or Quality Assurance System (SAC), migrating the system from serverjz to the Intranet and ensuring compliance with ISO9001:2015. The system must allow the creation, review, approval, distribution, and archiving of documents, guaranteeing traceability and regulatory compliance.

## Scope

- Review and analysis of the current system (documents and HTML).
- Design and implementation of a centralized and accessible solution on the Intranet.
- Implementation of version control, permissions, and change traceability.
- Compliance with ISO9001:2015.
- Prioritized migration of critical documents (policies, procedures, audits, etc.).

## Functional Requirements

- User control and role management (see User Roles and Permissions section).
- Document management: creation, review, approval, distribution, archiving, and deletion.
- Version management and change traceability.
- Advanced and efficient document search.
- Intuitive and user-friendly interface for users and administrators.
- Change tracking and process auditing.
- Secure and reliable access control to documents.
- Viewing, downloading, and consulting documents according to permissions.
- Chain approval management and document status control.
- Archiving and access to previous document versions.
- User manual and technical documentation.

### Manufacturing-Specific Functionalities

- Calibration management for measurement equipment (ISO9001:2015 7.1.5.2).
- Training and competency records for staff (ISO9001:2015 7.2).
- Management of non-conformities and corrective actions (ISO9001:2015 10.2).
- Control of changes in manufacturing and service processes (ISO9001:2015 8.5.6).
- Management of customer property (e.g., devices sent for testing) (ISO9001:2015 8.5.3).
- Design and development review records (if applicable) (ISO9001:2015 8.3).
- Supplier and external provider document management (for external audits).
- Audit module for internal and external audits (scheduling, findings, follow-up).

#### Example Use Cases

- Approval workflow for a new assembly procedure document.
- Registration and traceability of a non-conformity detected in production.
- Scheduling and documenting an internal or external audit.
- Assigning and tracking corrective actions after an audit.

## Non-Functional Requirements

- Information security and data backup.
- Integrity and authenticity of documents.
- Compatibility with modern browsers and existing systems.
- Adequate performance for large volumes of documents.
- Ease of maintenance, scalability, and updates.
- Access via Intranet or local network, without compromising confidentiality.
- Support for future integrations and APIs.
- Full compatibility and support for Windows Server 2019 environments.
- Automated backup and disaster recovery procedures.
- Detailed audit log for all relevant actions (for internal/external audits).
- Compliance with data protection and privacy regulations.

#### Example Non-Functional Scenarios

- The system must allow restoration of all documents and audit logs in case of server failure.
- All user actions (view, edit, approve, delete) must be traceable for at least 3 years.
- The system must support at least 50 concurrent users without performance degradation.

## User Roles and Access Levels

- **Level 1: Read-only user** – Views and downloads documents.
- **Level 2: Editor user** – Creates, edits, and downloads documents.
- **Level 3: Approver user** – Reviews and approves documents (first approval level).
- **Level 4: Document administrator** – Creates, edits, approves, deletes documents, and manages versions and auditing.
- **Level 5: System administrator** – Manages users, configures the system, and performs security audits.

## Permissions and Access Control

- Assignment of specific permissions by user level.
- Access control to functionalities according to role.
- Access to previous versions and control of document reliability and integrity.
- User management: creation, review, and approval.

## Standards and Regulations

- Compliance with ISO9001:2015 in all document management processes.
- Traceability, change management, and process auditing.

## Integrations and Dependencies

- Consider future integrations with other systems and document management tools.
- Identify technical and business dependencies to ensure compatibility and integration.

## Deliverables and Next Steps

- Definition of key dates and deliverables by phase.
- Assignment of responsibilities for each activity.
- Documentation of changes and version control.

## Success Criteria

- End-user satisfaction and meeting deadlines.
- Quality and compliance of generated documentation.
- Security, integrity, and system performance.
- Ability to handle large volumes of documents.
- Generation of reports and performance metrics.

## Risks and Limitations

- Identification of technical, resource, and time risks.
- Consideration of budget, human, and technological resource limitations.

## Communication and Follow-up

- Main channel: Slack Channel #qms-project
- Meeting frequency: To be defined.
- Change process: All changes must be documented and approved by the project team.

---

## Diagrams and Process Models

All diagrams are located in the folder `Docs/Diagrams/` and are provided in .drawio and .md formats for reference and editing.

### Suggested Diagrams:

- Use Case Diagram: Document Approval and Audit Management
- Class Diagram: Core Entities (User, Document, Audit, NonConformity, Equipment)
- Process Flow: Non-Conformity Management
- Architecture Diagram: QMS on Windows Server 2019

> See `Docs/Diagrams/` for templates and editable files.

---

**Additional Notes:**

- Analysis of the current SAC system and access to the server and repository are required for migration and version control.
- The system must be open to improvements and new functionalities without affecting current operations.
- Include a user manual and technical documentation for support and training.
- The system must be ready for both internal and external audits (by customers, suppliers, or certification bodies).
- All modules must support export of evidence and reports in PDF/Excel for audit purposes.
- The system should allow secure, temporary access for external auditors or clients when required.
- All process and class diagrams should be updated as the system evolves.
