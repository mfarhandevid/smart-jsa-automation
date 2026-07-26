Smart JSA Automation

An AI-assisted workflow automation system designed to streamline the Job Safety Analysis (JSA) process through WhatsApp-based communication, automated workflow orchestration, structured data management, and human-in-the-loop safety review.

Overview

Traditional JSA processes may involve multiple communication channels, manual data entry, document preparation, and sequential approval processes.

Smart JSA Automation is designed to connect these activities into a structured digital workflow.

The system allows a Supervisor to initiate a JSA request through WhatsApp and guides the request through job information collection, AI-assisted hazard analysis, Safety Officer review, HSSE Manager approval, registry updates, and final JSA document delivery.

The overall workflow is:

Supervisor
    ↓
WhatsApp Input
    ↓
Job Information Collection
    ↓
JSA Draft & AI-Assisted Hazard Analysis
    ↓
Safety Officer Review
    ↓
HSSE Manager Approval
    ↓
Approval & Registry Update
    ↓
Final JSA PDF Delivery

Key Concept

The system is designed around a human-in-the-loop approach.

AI assists with the initial analysis of potential hazards and safety considerations.

However, AI does not replace professional K3 judgment or organizational approval authority.

AI-Assisted Analysis
        ↓
Safety Officer Review
        ↓
HSSE Manager Approval
        ↓
Final JSA

The core principle is:

AI assists analysis. Qualified human personnel retain review and approval authority.

System Components

The system integrates several components:

WhatsApp — Primary communication interface.
n8n — Workflow orchestration layer.
AI — AI-assisted hazard analysis.
Google Sheets — Structured data and registry management.
Google Docs — JSA document generation.
PDF — Final document output and delivery.

These components are connected through an automated workflow.

Workflow

The workflow is organized into six major phases:

Phase 1 — Job Information Collection

The system communicates with the Supervisor to collect the information required to prepare the JSA.

Phase 2 — JSA Draft and AI-Assisted Hazard Analysis

The collected information is processed to prepare a JSA draft and support an initial AI-assisted hazard analysis.

Phase 3 — Safety Officer Review

The JSA draft and AI-assisted analysis are reviewed from a K3 perspective by the Safety Officer.

Phase 4 — HSSE Manager Review

The reviewed JSA proceeds to the HSSE Manager for management-level review and approval.

Phase 5 — Approval and Registry Update

The system updates the relevant approval records and JSA Registry.

Phase 6 — Final JSA PDF Delivery

The approved JSA is prepared as a final PDF and delivered through WhatsApp.

Repository Structure
smart-jsa-automation/
│
├── assets/
│   ├── diagrams/
│   └── screenshots/
│
├── docs/
│   ├── 01-project-overview.md
│   ├── 02-business-process.md
│   ├── 03-system-architecture.md
│   ├── 04-workflow-explanation.md
│   ├── 05-ai-and-k3-logic.md
│   └── 06-limitations-and-future-development.md
│
├── workflow/
│   └── README.md
│
└── README.md

Documentation

The project documentation is organized into several sections.

Project Overview

Explains the project background, objectives, and overall concept.

Business Process

Explains the roles and activities involved in the JSA workflow.

System Architecture

Explains how the major system components interact with one another.

Workflow Explanation

Explains the end-to-end workflow from WhatsApp input to final JSA delivery.

AI and K3 Logic

Explains the role of AI, human-in-the-loop design, and the boundary between AI-assisted analysis and human safety authority.

Limitations and Future Development

Explains the current limitations of the system and potential future development opportunities.

Visual Documentation

The repository includes visual documentation of the system design and workflow.

Visual assets may include:

System architecture diagrams.
End-to-end process diagrams.
Workflow screenshots.
Other selected visual documentation.

These assets provide additional context for understanding the system architecture and implementation concept.

Implementation Availability

The production workflow is not included in this public repository.

The repository is intended to document the system architecture, workflow design, AI and K3 logic, and development concept.

Production-specific implementation details are not publicly distributed.

This may include:

n8n workflow configurations.
AI prompt configurations.
Credentials and authentication settings.
Private data source references.
Organization-specific process logic.
Internal document structures.
Operational data.

The repository therefore functions as a public technical case study rather than a copyable production system.

Limitations

The system depends on:

The quality and completeness of the submitted job information.
The quality of AI-assisted analysis.
The availability of external integrations.
The accuracy of supporting data.
The defined organizational workflow.Human review and approval.

The automation does not replace professional K3 judgment or organizational safety governance.

Project Direction

Future development may explore:

Structured hazard and control libraries.
Organization-specific safety knowledge bases.
Retrieval-Augmented Generation.
Improved AI analysis support.
Dynamic information collection.
JSA analytics.
Workflow monitoring.
Advanced revision tracking.

The long-term direction is to develop a more intelligent and data-driven safety workflow platform while maintaining human oversight over critical safety decisions.

Disclaimer

This repository documents a technical project and system design concept.

The automation should be adapted to the applicable organizational procedures, safety management systems, legal requirements, and operational conditions before being used in a real-world environment.

AI-assisted analysis should not be treated as a replacement for qualified professional safety review.

Project Status

Status: Personal technical project / portfolio case study

Focus Areas:

Workflow automation.
AI-assisted analysis.
Occupational safety and health.
Human-in-the-loop system design.
Process digitization.
n8n workflow architecture.
