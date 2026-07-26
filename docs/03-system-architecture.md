System Architecture

Architecture Overview



Smart JSA Automation is built as an integrated workflow automation system that connects communication, workflow orchestration, AI-assisted analysis, data management, document generation, and approval processes.



The system uses WhatsApp as the primary communication interface, n8n as the workflow orchestration layer, Google Sheets as the structured data layer, AI as an analysis support component, and Google Docs as the document generation layer.



The overall architecture can be summarized as follows:



Supervisor

&#x20;   ↓

WhatsApp

&#x20;   ↓

n8n Workflow Automation

&#x20;   ├── User \& Request Validation

&#x20;   ├── Job Information Processing

&#x20;   ├── JSA Registry Lookup

&#x20;   ├── AI-Assisted Hazard Analysis

&#x20;   ├── Approval Routing

&#x20;   ├── Record Updates

&#x20;   └── Document Generation

&#x20;           ↓

&#x20;       Final JSA PDF

&#x20;           ↓

&#x20;       WhatsApp Delivery



Core Architecture Components

1\. User Interaction Layer



The user interaction layer is represented by WhatsApp.



It is used as the primary communication channel for:



* Initiating a JSA request.
* Providing job information.
* Receiving requests for additional information.
* Receiving review and approval-related notifications.
* Receiving the final approved JSA document.



The communication channel allows users to interact with the workflow without directly accessing the underlying automation infrastructure.



2\. Workflow Orchestration Layer



n8n acts as the central workflow orchestration layer.



It coordinates the interaction between the different system components and manages the overall JSA lifecycle.



The workflow orchestration layer is responsible for:



* Receiving incoming requests.
* Processing user and job information.
* Routing workflow execution.
* Interacting with data sources.
* Calling AI-assisted analysis.
* Managing approval stages.
* Updating records.
* Triggering document generation.
* Sending notifications and documents.



The workflow is organized into multiple phases that represent the major stages of the JSA process.



3\. Data Management Layer



Google Sheets is used as the structured data management layer.



The system uses structured records to support workflow operations such as:



* User validation.
* JSA registry management.
* Approval tracking.
* Workflow records.
* Audit and supporting data.



The data layer allows the automation to retrieve, update, and reference information throughout the JSA lifecycle.



4\. AI-Assisted Analysis Layer



The AI component supports the analysis of job information and potential hazards.



The AI-assisted analysis may support tasks such as:



* Identifying potential hazards.
* Structuring hazard information.
* Supporting risk analysis.
* Suggesting control measures.
* Producing structured analysis output for review.



The AI output is treated as an analytical aid rather than an independent approval mechanism.



The generated analysis is reviewed by the Safety Officer before the JSA proceeds through the approval workflow.



5\. Document Generation Layer



Google Docs is used to generate structured JSA documents based on the processed information.



The document generation process combines:



* Job information.
* JSA analysis.
* Hazard information.
* Risk controls.
* Required document fields.



The generated document is then prepared for review and approval.



After final approval, the completed JSA is delivered as a PDF document.



6\. Approval and Governance Layer



The approval layer introduces human review into the automated workflow.



The system routes the JSA through defined review stages:



AI-Assisted Analysis

&#x20;       ↓

Safety Officer Review

&#x20;       ↓

HSSE Manager Approval



This design ensures that the automation supports the workflow without removing human oversight from critical safety decisions.



High-Level Data Flow



The high-level data flow can be summarized as follows:



JSA Request

&#x20;   ↓

Job Information

&#x20;   ↓

JSA Draft

&#x20;   ↓

AI-Assisted Analysis

&#x20;   ↓

Safety Officer Review

&#x20;   ↓

HSSE Manager Approval

&#x20;   ↓

Registry Update

&#x20;   ↓

Final JSA PDF



The data is transformed as it moves through each stage of the workflow.



Component Interaction



The main system components interact as follows:



WhatsApp → n8n



The Supervisor submits a request and provides job information through WhatsApp.



The communication channel provides the input that initiates or continues the workflow.



n8n → Google Sheets



The workflow interacts with Google Sheets to:



* Validate users.
* Retrieve JSA-related records.
* Check registry information.
* Update approval status.
* Store relevant workflow information.



n8n → AI



The workflow sends relevant job information to the AI analysis component.



The AI processes the input and returns structured analysis that can be incorporated into the JSA workflow.



n8n → Google Docs



The workflow sends processed JSA information to the document generation layer.



The document generation process creates a structured JSA document based on the defined template and data.



n8n → WhatsApp



The workflow sends messages and documents back to the relevant users.



This may include:



* Requests for additional information.
* JSA draft notifications.
* Review notifications.
* Approval-related communication.
* Final approved JSA PDF delivery.



Architecture Principles



The system is designed around several principles.



Human-in-the-Loop



AI-assisted analysis is followed by human review and approval.



The system does not treat AI output as the final safety decision.



Modular Workflow



The automation is divided into separate functional stages.



Each stage has a specific responsibility within the overall JSA lifecycle.



This modular approach makes the workflow easier to understand, maintain, and improve.



Structured Data Management



The workflow uses structured records to manage users, JSA information, approval status, and registry information.



This allows the system to maintain consistent information across different workflow stages.



Communication-Driven Workflow



The system uses WhatsApp as the primary interaction layer.



This allows users to participate in the workflow through a familiar communication channel rather than requiring direct interaction with the underlying automation platform.



Separation of Responsibilities



Different actors maintain different responsibilities within the process:



* The Supervisor provides job information.
* The Smart JSA system processes and routes information.
* The Safety Officer performs technical K3 review.
* The HSSE Manager provides management-level approval.



This separation helps maintain accountability throughout the workflow.



Architecture Boundaries



The Smart JSA Automation system is designed to support the JSA workflow but does not replace:



* Professional K3 judgment.
* Organizational safety procedures.
* Management responsibility.
* Applicable legal and regulatory requirements.
* Site-specific safety controls.



The automation provides workflow coordination and analytical support, while final safety decisions remain subject to the applicable human review and approval process.

