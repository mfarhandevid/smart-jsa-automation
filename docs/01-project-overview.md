Smart JSA Automation

Overview



Smart JSA Automation is an AI-assisted workflow automation system designed to streamline the Job Safety Analysis (JSA) process from initial request to final document delivery.



The system combines WhatsApp-based communication, n8n workflow automation, AI-assisted hazard analysis, Google Sheets-based data management, Google Docs document generation, and multi-level review and approval.



The system is designed to support the collaboration between Supervisors, Safety Officers, HSSE Managers, and the automation system throughout the JSA lifecycle.



The Problem



Traditional JSA processes can involve multiple manual activities, including:



* Collecting job information from the requester.
* Identifying potential hazards.
* Developing risk controls.
* Reviewing JSA content.
* Coordinating approval between multiple stakeholders.
* Updating JSA records and approval status.
* Distributing the final approved document.



When these activities are handled manually across multiple communication channels and documents, the process may become time-consuming and difficult to track.



Smart JSA Automation addresses these administrative and coordination challenges by connecting the JSA workflow into a structured automation process.



The Solution



The system provides a structured workflow that connects:



WhatsApp Request

&#x20;       ↓

Job Information Collection

&#x20;       ↓

JSA Draft Generation

&#x20;       ↓

AI-Assisted Hazard Analysis

&#x20;       ↓

Safety Officer Review

&#x20;       ↓

HSSE Manager Approval

&#x20;       ↓

JSA Registry \& Approval Update

&#x20;       ↓

Final JSA PDF Delivery



The system is designed to reduce repetitive administrative work while maintaining human review and approval at critical stages of the JSA process.



Core Workflow



The Smart JSA Automation workflow consists of the following stages:



1\. WhatsApp Input



The Supervisor initiates the JSA request through WhatsApp.



2\. Job Information Collection



The system collects the information required to develop the JSA.



3\. JSA Draft Generation and AI-Assisted Analysis



The system generates a JSA draft based on the submitted job information and performs AI-assisted hazard analysis.



4\. Safety Officer Review



The draft JSA and AI-generated analysis are sent to the Safety Officer for technical K3 review and validation.



5\. HSSE Manager Review and Approval



After the Safety Officer's review, the JSA draft is submitted to the HSSE Manager for further review and approval.



6\. Record Update and Final Delivery



The system updates the relevant approval and JSA registry records. After final approval, the approved JSA is delivered as a PDF through WhatsApp.



Key Components



WhatsApp

Acts as the primary communication interface for:



* Submitting JSA requests.
* Collecting job information.
* Communicating review and approval actions.
* Delivering the final approved JSA document.



n8n

Acts as the workflow orchestration layer that connects the different components of the system.



It manages:



* Workflow routing.
* Data processing.
* User validation.
* Communication logic.
* JSA registry interactions.
* AI integration.
* Document generation.
* Approval status updates.
* AI-Assisted Analysis



AI is used to support the initial analysis of potential hazards and safety considerations based on the submitted job information.



The AI output is treated as an analytical aid and does not replace the responsibility of qualified human safety professionals.



Google Sheets



Used as a structured data layer for managing information such as:



* User data.
* JSA registry records.
* Approval status.
* Audit records.
* Supporting reference data.
* Google Docs



Used as the document generation layer for creating structured JSA documents.



PDF



The final approved JSA is delivered as a PDF document through WhatsApp.



Human-in-the-Loop Design



A key principle of the system is that AI does not independently provide final safety approval.



The workflow maintains human involvement at critical decision points:



AI-Assisted Analysis

&#x20;       ↓

Safety Officer Review

&#x20;       ↓

HSSE Manager Approval



This design allows AI to support repetitive analytical and administrative tasks while retaining human authority over professional safety review and final approval.



Intended Benefits



The system is designed to:



* Reduce repetitive administrative activities.
* Structure the JSA request and review process.
* Support AI-assisted hazard identification.
* Improve visibility of JSA approval status.
* Centralize JSA registry updates.
* Improve document traceability.
* Streamline communication between stakeholders.
* Deliver approved JSA documentation through an existing communication channel.



Project Scope

This project focuses on automating the workflow surrounding the JSA lifecycle, including:



* Request initiation.
* Job information collection.
* Draft JSA generation.
* AI-assisted hazard analysis.
* Safety Officer review.
* HSSE Manager approval.
* Registry and approval record updates.
* Final document delivery.



The system is intended to support the JSA process and does not replace professional safety judgment, organizational procedures, or applicable occupational safety requirements.



Project Status



This project is an ongoing portfolio and technical development project.



The repository presents the system architecture, workflow design, documentation, selected implementation examples, and technical approach.



Production-specific prompts, templates, credentials, operational data, and other sensitive implementation details may be excluded from the public repository.



Technology Stack

* n8n — Workflow automation and orchestration
* WhatsApp — User interaction and communication channel
* AI — Assisted hazard analysis
* Google Sheets — Data and registry management
* Google Docs — JSA document generation
* PDF — Final document delivery
* Docker — Local development environment



Repository Structure

smart-jsa-automation/

│

├── assets/

├── docs/

├── examples/

├── notes/

├── prompts/

├── templates/

├── workflow/

│

└── README.md



Further technical details about the business process, system architecture, workflow implementation, data structure, and AI logic are documented in the corresponding files within the docs/ directory.

