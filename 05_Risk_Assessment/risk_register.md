# HDIIA Critical Infrastructure Security Assessment

# Risk Register

Version: 1.0

Phase: 05 Risk Assessment

---

# Ελληνική Έκδοση

## 1. Σκοπός

Το Risk Register αποτελεί το κύριο artifact της φάσης Risk Assessment.

Βασίζεται στα:

- Business Services Catalog
- Asset Inventory Register
- Asset Dependency Matrix
- Threat Scenario Register
- Risk Assessment Methodology

Στόχος είναι η μετατροπή των threat scenarios σε αξιολογημένους επιχειρησιακούς κινδύνους.

---

# 2. Risk Register Model

Η σχέση αξιολόγησης:

Business Service

↓

Asset

↓

Dependency

↓

Threat Scenario

↓

Risk

↓

Control Treatment

---

# 3. Risk Register

| Risk ID | Threat Scenario Reference | Affected Asset | Business Service | Threat Actor | Likelihood | Impact | Risk Level | Risk Owner | Existing Controls | Recommended Treatment |
|---|---|---|---|---|---|---|---|---|---|---|
| R-001 | TS-001 Ransomware Attack | Application Platform | Critical Applications | Cyber Criminal Group | Medium | High | High | Application Owner | Endpoint Protection, Backup Controls | Improve segmentation, recovery testing, ransomware protection |
| R-002 | TS-002 Credential Compromise | Identity Infrastructure | Identity and Access Management | External Threat Actor | High | High | Critical | Identity Owner | Access Control, Authentication Policies | Enforce MFA, privileged access management |
| R-003 | TS-003 Privileged Account Misuse | Administrative Accounts | Infrastructure Operations | Insider User | Low/Medium | High | High | Security Manager | Account Monitoring | Strengthen privileged access governance and auditing |
| R-004 | TS-004 Supply Chain Compromise | External Dependencies | Critical Services | Third Party | Low | High | High | Vendor Owner | Supplier Management | Improve third-party risk assessment |
| R-005 | TS-005 Network Disruption | Core Network Services | Infrastructure Services | Cyber Actor / Failure | Medium | Medium/High | High | Infrastructure Owner | Network Monitoring | Increase resilience and redundancy |

---

# 4. Risk Ownership

Κάθε κίνδυνος πρέπει να έχει:

- Risk Owner
- Business Owner
- Technical Owner
- Treatment Responsibility

---

# 5. Risk Treatment Preparation

Οι προτεινόμενες ενέργειες θα χρησιμοποιηθούν για:

- Security Control Mapping
- Risk Treatment Plan
- Improvement Roadmap

---

# English Version

## Purpose

The Risk Register documents evaluated risks derived from identified threat scenarios.

It connects:

- Business services
- Assets
- Dependencies
- Threat scenarios
- Security treatments

---

## Risk Evaluation Model

Business Service

↓

Asset

↓

Dependency

↓

Threat Scenario

↓

Risk

↓

Control Treatment

---

## Risk Management Usage

The register provides input for:

- Security Control Mapping
- Risk Treatment Planning
- Security Improvement Roadmap

---

# Document Status

Current Phase:

05 Risk Assessment

Next Phase:

06 Security Control Mapping
