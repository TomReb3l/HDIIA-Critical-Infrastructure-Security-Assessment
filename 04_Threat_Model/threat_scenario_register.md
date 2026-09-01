# HDIIA Critical Infrastructure Security Assessment

# Threat Scenario Register

Version: 1.0
Phase: 04 Threat Model

# Ελληνική Έκδοση

## 1. Σκοπός

Το Threat Scenario Register αποτελεί το επιχειρησιακό αποτέλεσμα της φάσης Threat Modeling.

Βασίζεται στα προηγούμενα artifacts:
- Business Services Catalog
- Asset Inventory Register
- Asset Dependency Matrix
- Threat Model Methodology

Στόχος είναι η καταγραφή ρεαλιστικών σεναρίων απειλών που επηρεάζουν κρίσιμες υπηρεσίες, assets και dependencies.

## 2. Threat Scenario Identification Model

Threat Actor → Attack Path → Target Asset → Business Service Impact → Risk Assessment

## 3. Threat Scenario Register

| ID | Threat Scenario | Threat Actor | Target Asset | Business Impact | Attack Path | Likelihood | Impact |
|---|---|---|---|---|---|---|---|
| TS-001 | Ransomware attack against critical application infrastructure | Cyber Criminal Group | Application Platform | Service interruption | Malware execution and encryption | Medium | High |
| TS-002 | Credential compromise against identity infrastructure | External Threat Actor | Identity Infrastructure | Unauthorized access | Phishing and credential theft | High | High |
| TS-003 | Privileged account misuse | Insider User | Administrative Accounts | Confidentiality and integrity impact | Privileged access abuse | Low/Medium | High |
| TS-004 | Supply chain compromise | Third Party | External Dependencies | Service disruption | Trusted access abuse | Low | High |
| TS-005 | Network infrastructure disruption | Cyber Actor / Failure | Core Network Services | Availability degradation | Attack or failure | Medium | Medium/High |

## 4. Existing Security Considerations

- Identity and Access Management
- Multi-Factor Authentication
- Network Segmentation
- Endpoint Protection
- Security Monitoring
- Backup and Recovery
- Supplier Security Controls

## 5. Risk Assessment Preparation

Threat scenarios provide input for likelihood, impact, risk scoring and security control selection.

# English Version

## Purpose

The Threat Scenario Register documents realistic threat scenarios affecting critical services, assets, and dependencies.

## Risk Assessment Preparation

Threat scenarios provide input for:
- Likelihood analysis
- Impact evaluation
- Risk scoring
- Security control selection

# Document Status

Current Phase: 04 Threat Model

Next Phase: 05 Risk Assessment
