---
name: fitness-project-synopsis
description: Create or revise a 15-20 page LaTeX project-proposal synopsis for the Formwell fitness tracking system. Use when asked to write, update, or compile the project's academic proposal/synopsis seeking formal approval to proceed with building the project.
---

# Fitness Project LaTeX Synopsis (Project Proposal for Approval)

Create a complete, academically rigorous LaTeX project synopsis for the Formwell fitness tracking and activity monitoring system. This document serves as the **initial project proposal submitted to the academic review committee, faculty guide, and department for formal approval to proceed with building the project**.

The document must read prospectively as a thorough, professional proposal—articulating the problem, proposed solution, objectives, system requirements, architectural design, database modeling, methodology, security design, and execution schedule. Ground the technical specifications in the system design, models, and prototypes in `../frontend-fitness` and `../backend-fitness`, framing them as concrete engineering specifications for the system to be developed.

## Workflow and Framing Principles

1. **Prospective Proposal Framing**: The synopsis must be framed as a document submitted for **project approval prior to full-scale development**. Use prospective/proposal language throughout ("The proposed system will provide...", "The project aims to design and implement...", "The planned architecture consists of...", "Proposed functional requirements...", "Planned development phases..."). Avoid framing the document as a retrospective audit, code review, or post-completion inspection of an existing codebase.
2. **Grounding in Concrete System Design**: Leverage the architectural models, API structures, frontend flows, and database designs from `frontend-fitness` and `backend-fitness` to ensure the proposal contains concrete, realistic engineering details (exact entity relationships, data flow diagrams, route specifications, and component interactions), rather than vague abstractions.
3. **Engineering Rigor & Best Practices**: Present architectural decisions, security controls (such as adaptive password hashing via bcrypt, stateless JWT bearer token authentication, token-derived subject authorization, and strict server-side validation), database normalization, and data-integrity constraints as the **proposed technical specifications and design standards** of the project to be built.
4. **Academic Document Structure**: Target a polished 15–20 page document using standard academic report layout, a formal title page with institutional placeholders, an abstract/executive summary, a formal submission note, table of contents, list of figures, list of tables, numbered chapters, clear TikZ diagrams, comprehensive schema tables, and formal citations.
5. **Legible Native Diagrams**: Use clean, legible TikZ diagrams for Level-0/1/2 DFDs, Entity-Relationship (ER) model, Activity Diagram, Class/Component Architecture, State Machine Diagram, Deployment Topology, Gantt Chart, and PERT Precedence Network.
6. **Compilation Verification**: When a LaTeX compiler (`pdflatex` or `latexmk`) is available, compile the document to verify there are no compilation errors, missing citations, or broken references, ensuring a high-quality PDF is generated.

## Required Synopsis Content

The proposal must include the following 13 comprehensive sections:

1. **Title Page and Submission Statement**: Formal title page with project title, subtitle, degree/program, student details, guide, department, institution placeholders, and a formal submission note requesting approval to undertake the proposed project.
2. **Abstract and Executive Summary**: Overview of the proposed personal fitness tracking system, core problem addressed, proposed technological solution, key planned capabilities, and significance.
3. **Introduction and Objectives**: Background context, motivation, target user demographic, problem definition, and measurable project objectives.
4. **Project Category and Technical Domain**: Classification (RDBMS-based web application, modular software architecture, web networking) with technical justification. Clarify scope boundaries (e.g., deterministic rule-based plan categorization rather than predictive AI/ML).
5. **Scope of the Proposed Solution**: Clear delineation of in-scope capabilities for the approved project lifecycle, explicit out-of-scope boundaries, design assumptions, and environmental constraints.
6. **Literature Review and Theoretical Foundation**: Review of relevant domain literature (e.g., WHO physical activity guidelines), open standards (RFC 7519 JWT), architectural frameworks (relational persistence, GORM ORM), and security baselines (OWASP password storage and authentication guidelines).
7. **System Requirements Specification**: Detailed proposed Functional Requirements (FR) using standard requirement specifications ("The system shall..."), and Non-Functional Requirements (NFR) covering security, data integrity, usability, maintainability, portability, and privacy.
8. **System Analysis and Architectural Models**:
   - Level-0 Context DFD
   - Level-1 System DFD
   - Level-2 Detailed DFD (Core Daily Activity Tracking & Logging Workflow)
   - Entity-Relationship (ER) Diagram with entity cardinalities
   - Activity Diagram illustrating end-to-end user workflows
   - High-Level Class / Component Diagram
   - State Transition Diagram for daily activity recording
9. **Proposed Database Design**: Comprehensive data dictionary and relational schema tables (User, Daily Activity & Targets, Category Lookups, Mapping, Workout & Diet Schedules), primary and foreign keys, integrity constraints, normalization analysis, and audit design.
10. **Modular Structure and Implementation Methodology**: Decomposition into functional modules (Identity & Authentication, Profile & Baseline Assessment, Plan Recommendation Engine, Daily Activity Logging, Progress Analytics & Reporting, Core API & Persistence), planned process logic, core data structures, and planned reports.
11. **Network and Deployment Architecture**: Proposed client-server deployment topology, containerized database environment, API communication protocols, and security trust boundaries.
12. **Security Architecture and Planned Controls**: Multilayered security design covering authentication, token-bound authorization, credential hashing, transport encryption, CORS policy, input validation, and privacy protection.
13. **Project Planning, Scheduling, and Risk Analysis**:
    - Project development phases and methodology
    - Relative 8-week Gantt Chart
    - PERT Precedence Network and critical path analysis
    - Risk assessment matrix with proactive mitigation strategies
14. **Expected Outcomes, Deliverables, and Conclusion**: Anticipated project deliverables, expected impact, and concluding approval appeal.
15. **Academic References / Bibliography**: Formal citations of standards, literature, and architectural references.

## Completion Report

When complete, confirm the updated source, verify that all retrospective/audit language has been transformed into prospective proposal framing suitable for committee approval, report compiler results (page count and PDF status), and summarize any key placeholders or assumptions.