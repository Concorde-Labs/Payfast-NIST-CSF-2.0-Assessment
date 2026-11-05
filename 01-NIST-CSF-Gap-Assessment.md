# Payfast Inc.
## NIST CSF 2.0 - Cybersecurity Gap Assessment

**Prepared by:** Concord Ekwonna  
**Framework:** NIST Cybersecurity Framework 2.0  
**Supporting Reference:** NIST SP 800-53 Rev. 5  
**Assessment Status:** Preliminary

---

## 1. Executive Summary

Payfast Inc. is a fintech company providing digital payment services to individuals and small businesses. The organization employs approximately 180 people and relies on cloud-hosted applications, employee devices, internal systems, and external APIs.

Although Payfast has established some cybersecurity practices, these are managed inconsistently across departments. Identified weaknesses include decentralized asset inventories, unclear security responsibilities, inconsistent access management, limited security monitoring, and insufficiently formalized incident response and recovery arrangements.

This assessment applies NIST CSF 2.0 to evaluate Payfast's current cybersecurity practices, define desired security outcomes, identify gaps, and recommend areas for improvement.

Five core business processes were assessed, with findings mapped to relevant NIST SP 800-53 control families.

## 2. Assessment Scope and Methodology

The assessment covers the following business processes:

1. Customer Onboarding & Account Management
2. Payment Processing
3. Asset & System Management
4. Employee Access Management
5. Third-Party Payment Integrations

The assessment approach involved reviewing documented cybersecurity practices, mapping relevant NIST CSF 2.0 functions, establishing preliminary Current and Target Profiles, identifying gaps, and selecting supporting SP 800-53 control families.

**Assessment limitation:** The analysis is based on a provided organizational case study. No independent technical testing, interviews, or control effectiveness reviews were performed.

## 3. NIST CSF 2.0 Current and Target Profile Gap Analysis

| Business Process | Relevant CSF 2.0 Function(s) | Current Profile | Target Profile | Identified Gap | Relevant SP 800-53 Control Family |
|---|---|---|---|---|---|
| Customer Onboarding & Account Management | Protect (PR) | MFA is implemented on some systems and accounts but is not consistently applied. | Appropriate authentication safeguards, including MFA, are consistently implemented across relevant customer-facing systems. | Inconsistent authentication protection may increase unauthorized account access exposure. | IA - Identification and Authentication |
| Payment Processing | Detect (DE), Recover (RC) | Security monitoring is inconsistent across critical systems; recovery procedures are not formally documented or regularly tested. | Critical payment systems are monitored for suspicious activity, with documented and tested recovery procedures. | Limited detection capability and insufficient recovery preparedness. | AU - Audit and Accountability; CP - Contingency Planning |
| Asset & System Management | Identify (ID) | Departments maintain separate asset records without a centralized inventory. | A centralized, maintained inventory provides visibility of important systems and information assets. | Limited organization-wide asset visibility and ownership. | CM - Configuration Management |
| Employee Access Management | Protect (PR) | Employee access rights are not consistently reviewed following role changes; MFA coverage is inconsistent. | Access privileges are reviewed promptly following role changes and appropriate authentication controls are enforced. | Excessive privileges and inconsistent authentication safeguards. | AC - Access Control; IA - Identification and Authentication |
| Third-Party Payment Integrations | Govern (GV), Respond (RS) | Third-party cybersecurity responsibilities and incident-handling arrangements are not formally established. | Supplier security responsibilities are documented, and third-party incident reporting and response arrangements are defined. | Weak third-party security governance and incident coordination. | SR - Supply Chain Risk Management; IR - Incident Response |

### Additional Cross-Cutting Findings

The case study also identifies weaknesses that affect multiple business processes:

- **Cybersecurity governance:** Security responsibilities and risk management processes are not consistently defined across departments.
- **Security awareness:** Employees receive onboarding training without regular refresher sessions.
- **Incident response:** Payfast lacks a consistent organization-wide incident management process.

These weaknesses should be addressed through the framework implementation plan rather than treated as isolated business-process issues.

## 4. Preliminary Risk Prioritization

The following priorities reflect the potential business consequences of identified weaknesses. They are preliminary judgments rather than formal risk scores.

| Finding | Preliminary Priority | Business Risk Rationale |
|---|---|---|
| Inconsistent monitoring and recovery preparedness | High | Delayed detection and ineffective recovery could disrupt critical payment services. |
| Inconsistent employee access reviews and authentication | High | Unnecessary privileges and weak authentication may expose sensitive systems and information. |
| Undefined third-party security responsibilities | High | Supplier-related incidents may be difficult to coordinate and manage. |
| Decentralized asset inventory | Medium | Limited asset visibility may prevent consistent protection and risk assessment. |
| Inconsistent customer-facing
