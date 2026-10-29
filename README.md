# Nexus Health Services | PCI DSS & HIPAA Compliance Assessment

![Project](https://img.shields.io/badge/Project-GRC%20Case%20Study-blue)
![Sector](https://img.shields.io/badge/Sector-Healthcare-008080)
![Focus](https://img.shields.io/badge/Focus-PCI%20DSS%20%26%20HIPAA-005A9C)
![Deliverable](https://img.shields.io/badge/Deliverable-Assessment%20Report-grey)

A documentation-based governance, risk, and compliance project examining how a healthcare organization can protect payment card data and patient information.

The assessment connects critical business processes, sensitive-data flows, compliance boundaries, risks, controls, evidence requirements, and remediation priorities. It concludes with an executive-level explanation of the three most urgent risks.

> Educational case study. This project contains analysis and recommendations, not a completed compliance audit, implemented security solution, or formal PCI DSS or HIPAA compliance determination.

## Project Overview

Nexus Health Services is a multi-site healthcare organization operating hospitals, outpatient clinics, and diagnostic centers.

It accepts payment cards through in-person transactions and an online patient portal while handling protected health information through clinical, billing, support, and vendor workflows.

Management’s central question is:

> How can Nexus demonstrate that it adequately protects payment card data and health information?

This project answers that question by tracing the relationship between business activities, regulated information, applicable requirements, and evidence of control effectiveness.

## Problem Statement

The assessment identifies five principal case-study gaps:

- Weak privileged authentication
- Security logs that are collected but not reviewed
- A healthcare vendor operating without a documented Business Associate Agreement
- Incomplete or unvalidated compliance scope
- An unclear and untested incident-response process

It also evaluates additional scenarios involving device loss, inadequate payment-data protection, and policies that are not consistently followed.

These weaknesses could expose Nexus to unauthorized access, data breaches, delayed detection, fraud, operational disruption, and regulatory or contractual consequences.

## Project Objectives

- Identify critical business processes and their business impact.
- Map sensitive information, systems, flows, and access roles.
- Distinguish PCI DSS and HIPAA assessment boundaries.
- Develop a qualitative risk map.
- Connect risks to relevant requirements and proposed controls.
- Define the evidence needed to evaluate control implementation and operation.
- Prioritize remediation.
- Communicate the most urgent risks to leadership in plain language.

## Key Deliverables

| Deliverable | Included Analysis |
|---|---|
| Business scope | Five critical processes and their business impact |
| Data map | Information types, systems, destinations, and access roles |
| Compliance scope | Separate PCI DSS and HIPAA scoping considerations |
| Risk map | Eight risk scenarios with qualitative likelihood, impact, and ratings |
| Control mapping | Proposed controls associated with PCI DSS requirements and HIPAA safeguard areas |
| Evidence plan | Requested artifacts, responsible owners, and intended assurance |
| Remediation plan | Eight prioritized actions with completion evidence |
| Management message | Executive explanation of the three most urgent risks |

The central strength of the project is its traceability: each recommendation connects back to a business process, data exposure, risk, or evidence need.

## Assessment Workflow

```text
Business Processes
        |
        v
Sensitive Data and Data Flows
        |
        v
PCI DSS and HIPAA Scope
        |
        v
Risk Scenarios and Priorities
        |
        v
Requirements and Proposed Controls
        |
        v
Evidence and Control Evaluation
        |
        v
Remediation and Management Reporting
```

The assessment proposes a shared control layer while maintaining distinct payment-data and health-information scopes.

For example, authentication, monitoring, vendor governance, and incident-response activities may support more than one obligation. Their applicability still needs to be evaluated separately for each environment and requirement.

## Business Processes Assessed

| Process | Information or Activity Examined | Business Concern |
|---|---|---|
| Payment processing | In-person POS transactions, portal payments, and payment-gateway flows | Payment-data exposure and disruption to card acceptance |
| Healthcare billing and claims | Patient identifiers, treatment information, insurance details, and billing records | Privacy breaches and inappropriate disclosure |
| Patient support | Identity and account queries, CRM records, recordings, and screen captures | Exposure of patient information or payment details |
| Account management | Balances, refunds, bank details, and settlement records | Fraud and unauthorized financial activity |
| Vendor management | Contracts, vendor access, security assessments, and business associate arrangements | Third-party misuse or inadequate protection of regulated information |

## Data and Compliance Scope

The report distinguishes between:

- Payment account data handled through payment workflows
- PHI and ePHI handled through healthcare and supporting workflows
- Other sensitive financial, identity, and vendor information

Systems discussed include:

- Point-of-sale terminals
- Online patient portal
- Payment gateway
- Electronic health record system
- Billing system
- Customer relationship management system
- Banking platform
- Cloud services
- Vendor portal and contract repository

The data map describes information that may be handled during business processes. It does not establish that every listed data element is retained or that any particular storage practice is permitted.

Actual compliance boundaries require validation of data flows, system connectivity, vendor responsibilities, and technical safeguards.

## Risk Assessment Summary

Ratings below reflect the report’s qualitative assessment, not independently tested results.

| ID | Risk Scenario | Rating |
|---|---|---|
| R1 | Weak privileged authentication permits unauthorized access | Critical |
| R2 | Unreviewed logs delay detection and investigation | Critical |
| R3 | A healthcare vendor lacks a documented Business Associate Agreement | High |
| R4 | Incomplete scope leaves relevant systems or vendors outside the assessment | High |
| R5 | Untested incident response leads to ineffective containment or escalation | High |
| R6 | A lost laptop or mobile device exposes ePHI | High |
| R7 | Inadequately protected payment data is accessed or disclosed | High |
| R8 | Policies exist but are not followed in practice | High |

The first five findings are presented as principal gaps in the report. The remaining risks broaden the analysis to additional security scenarios.

## Proposed Controls and Evidence

| Control Area | Proposed Improvement | Example Evidence Requested |
|---|---|---|
| Authentication and access | Individual accounts, role-based access, stronger authentication, MFA, and access reviews | Access reports, configuration records, and MFA evidence |
| Security monitoring | Centralized logging, assigned reviewers, anomaly investigation, and documented review | Log-review records, monitoring reports, and investigation records |
| Vendor governance | Review applicable agreements, execute required BAAs, and assess vendor security | Signed agreements, security assessments, and responsibility records |
| Compliance scoping | Validate processes, data flows, systems, users, and third parties | Approved scope, process inventory, and data map |
| Incident response | Define roles, escalation, recovery activities, and exercises | Approved plan, exercise results, and corrective actions |
| Physical and device security | Device tracking, workstation protection, facility controls, and secure disposal | Inventories, access records, and disposal evidence |
| Data protection | Minimize retained payment information and protect data at rest and in transit | Configuration records and protection test results |
| Security awareness | Role-based training and periodic evaluation | Training materials, completion records, and evaluation results |

These artifacts are requested evidence. The repository does not contain collected evidence proving that the controls operate effectively.

## Prioritized Remediation

### Immediate

1. Strengthen authentication and privileged-access protection.
2. Establish accountable security-log review and investigation.

### High Priority

3. Review vendor arrangements and execute the required BAA.
4. Validate PCI DSS and HIPAA assessment scopes.
5. Document and exercise incident response.
6. Strengthen physical and device security.
7. Improve stored and transmitted data protection.
8. Deliver role-based security and privacy training.

The report provides a proposed sequence and completion evidence. It does not include confirmed budgets, implementation dates, or completed remediation results.

## Executive Communication

The management summary concentrates on three connected concerns:

- Weak authentication can allow stolen credentials to expose sensitive systems.
- Unreviewed logs can allow unauthorized activity to continue without timely investigation.
- Missing business associate agreements leave vendor responsibilities insufficiently documented.

This translates technical and compliance findings into business decisions about access protection, detection capability, and third-party accountability.

## Tools, Formats, and Technologies

| Item | Role |
|---|---|
| DOCX | Assessment report format |
| Markdown | Repository documentation |
| PCI DSS | Payment-data security reference used in the assessment |
| HIPAA | Healthcare privacy and security requirements discussed in the report |
| Qualitative risk assessment | Method used to prioritize scenarios |
| Data mapping | Method used to connect processes, information, systems, and access |

The systems described in the case study are assessment subjects, not technologies deployed by this project.

No programming language, application runtime, database product, cloud vendor, SIEM product, or automated testing tool is confirmed in the supplied material.

## Repository Structure

Suggested layout:

```text
.
├── README.md
└── Assignment-on-PCI_DSS-HIPAA.docx
```

## Getting Started

### Prerequisites

- A DOCX-compatible document viewer
- Git, only if cloning the repository

No application installation, cloud credentials, package dependencies, or build steps are required.

### Review the Report

Download `Assignment-on-PCI_DSS-HIPAA.docx` from the repository and open it in a compatible viewer.

Alternatively, replace the placeholders and clone the repository:

```bash
git clone [https://github.com/](https://github.com/)<github-username>/<repository-name>.git
cd <repository-name>
```

Open the DOCX report to review the full assessment.

## Usage

### For Recruiters and Hiring Managers

Review the report to evaluate:

- Healthcare and payment-data risk analysis
- Business-process and sensitive-data mapping
- Compliance scoping
- Requirement-to-control traceability
- Evidence planning
- Remediation prioritization
- Executive communication

### For Learners and Reviewers

1. Start with the business scope and data map.
2. Trace each risk to the proposed control.
3. Review what evidence would be needed to evaluate implementation and effectiveness.
4. Examine the remediation sequence and management message.
5. Identify assumptions that would require validation in a real assessment.

Before operational use, validate the applicable PCI DSS version, detailed requirement mappings, HIPAA applicability, contractual obligations, and organization-specific evidence.

## Limitations

- The assessment is based on a case-study narrative.
- No live-system testing, interviews, configuration validation, or evidence collection is documented.
- Risk ratings are qualitative; a detailed numerical scoring model is not supplied.
- Requirement mappings are primarily at the PCI DSS requirement and HIPAA safeguard level.
- The report does not establish an actual PCI DSS validation pathway.
- Proposed controls are not demonstrated as implemented or effective.
- The analysis is not legal advice or a formal compliance determination.

## Future Enhancements

Potential additions—not currently supplied—include:

- Visual data-flow and environment diagrams
- Detailed PCI DSS subrequirement and HIPAA citation mapping
- Risk-scoring criteria and acceptance thresholds
- Control and evidence register
- Vendor responsibility matrix
- Remediation tracker with owners and target dates
- Incident-response exercise template
- Executive dashboard
- PDF version of the report
- Screenshots of completed supporting templates using synthetic data

## Contributing

To propose a correction or enhancement:

1. Open an issue describing the change and supporting rationale.
2. Keep case-study facts separate from assumptions.
3. Submit focused changes through a pull request.
4. Explain any changes to regulatory mappings or risk ratings.

Do not upload real patient records, payment card details, credentials, confidential vendor agreements, or other sensitive information.

Use synthetic examples for any additional templates or screenshots.

## Author

Maureen Uzoewulu  
GRC Analyst — Case-Study Portfolio

- GitHub: <GitHub profile URL>
- LinkedIn: <LinkedIn profile URL>
- Contact: <optional professional email>

## References

The source report cites:

- 10Alytics course materials on PCI DSS and HIPAA
- LoginTC material on PCI DSS authentication
- Secure60 material on logging and review
- HIPAA Journal material on business associate agreements and breach notification

See the report for full reference details. Validate consequential regulatory interpretations against applicable authoritative sources before operational use.

## License

<Specify reuse permissions and add a corresponding LICENSE file if appropriate.>

Distinguish original project content from third-party course materials and other copyrighted sources.
