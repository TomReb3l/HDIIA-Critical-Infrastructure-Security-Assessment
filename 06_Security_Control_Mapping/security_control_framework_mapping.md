# HDIIA Critical Infrastructure Security Assessment

# Security Control Framework Mapping

**Version:** 1.1\
**Phase:** 06 Security Control Mapping\
**Status:** Final Hardening --- Risk to Control Traceability

------------------------------------------------------------------------

# Ελληνική Έκδοση

## 1. Σκοπός Control Mapping

Το Security Control Framework Mapping αποτελεί τη σύνδεση μεταξύ των
αξιολογημένων κινδύνων και των απαιτούμενων security controls.

Βασίζεται στα:

-   Risk Register
-   Threat Scenario Register
-   Asset Inventory Register
-   Asset Dependency Matrix
-   Risk Assessment Methodology

Στόχοι:

-   αντιστοίχιση risks με security controls,
-   τεκμηρίωση control requirements,
-   υποστήριξη Target Security Architecture,
-   δημιουργία traceability μεταξύ risk, control και implementation
    requirement.

------------------------------------------------------------------------

# 2. Risk to Control Traceability Model

Η σχέση ακολουθεί:

Risk

↓

Security Objective

↓

Security Control

↓

Framework Reference

↓

Architecture Requirement

↓

Implementation Activity

------------------------------------------------------------------------

# 3. Risk Based Control Mapping

  --------------------------------------------------------------------------------------
  Risk ID     Risk         Security         Required         NIST CSF    ISO/IEC
              Scenario     Objective        Controls         2.0         27001:2022
                                                             Alignment   Alignment
  ----------- ------------ ---------------- ---------------- ----------- ---------------
  R-001       Ransomware   Protect critical Endpoint         Protect,    A.8.13 Backup,
              Attack       applications and Protection,      Detect,     A.8.8
                           improve          Backup, Network  Recover     Vulnerability
                           resilience       Segmentation,                Management
                                            Recovery Testing             

  R-002       Credential   Protect identity MFA, PAM, Least  Govern,     A.5.15 Access
              Compromise   and access       Privilege,       Protect,    Control, A.5.16
                                            Authentication   Detect      Identity
                                            Monitoring                   Management

  R-003       Privileged   Control          Privileged       Govern,     A.8.2
              Account      administrative   Access           Protect,    Privileged
              Misuse       access           Management,      Detect      Access Rights
                                            Account                      
                                            Monitoring,                  
                                            Audit Logging                

  R-004       Supply Chain Manage           Supplier         Govern,     A.5.19 Supplier
              Compromise   third-party      Assessment,      Identify    Relationships
                           security         Third Party Risk             
                           exposure         Management                   

  R-005       Network      Maintain         Segmentation,    Protect,    A.8.14
              Disruption   availability and Monitoring,      Detect,     Redundancy of
                           operational      Redundancy,      Recover     Processing
                           resilience       Recovery                     Facilities
                                            Procedures                   
  --------------------------------------------------------------------------------------

------------------------------------------------------------------------

# 4. Security Control Categories

## Identity and Access Management

Controls:

-   Multi-Factor Authentication
-   Least Privilege Access
-   Privileged Access Management
-   Identity Monitoring

## Network Security

Controls:

-   Network Segmentation
-   Firewall Controls
-   Secure Network Architecture
-   Network Monitoring

## Data Protection

Controls:

-   Encryption
-   Backup Protection
-   Data Access Control
-   Recovery Procedures

## Security Monitoring

Controls:

-   SIEM
-   Centralized Logging
-   Detection Rules
-   Incident Response

## Resilience and Recovery

Controls:

-   Disaster Recovery
-   Business Continuity
-   Redundancy
-   Recovery Testing

------------------------------------------------------------------------

# 5. NIST CSF 2.0 Alignment

The mapping considers the six NIST CSF 2.0 Functions:

  Function   Security Focus
  ---------- ----------------------------------------------
  Govern     Risk strategy, policies, supplier governance
  Identify   Assets, risks, dependencies
  Protect    Access control, protection mechanisms
  Detect     Monitoring and event detection
  Respond    Incident response and containment
  Recover    Recovery and resilience

------------------------------------------------------------------------

# 6. ISO/IEC 27001:2022 Alignment

The mapping references relevant control themes:

-   Access Control
-   Identity Management
-   Asset Management
-   Supplier Security
-   Backup and Recovery
-   Operations Security
-   Incident Management
-   Business Continuity

This mapping supports control alignment and traceability. It does not
represent certification or compliance attestation.

------------------------------------------------------------------------

# 7. Control Implementation Principles

Controls are selected based on:

-   Risk priority
-   Business impact
-   Asset criticality
-   Operational requirements
-   Security maturity

------------------------------------------------------------------------

# English Version

## Purpose

Security Control Framework Mapping connects evaluated risks with
required security controls, framework references, and implementation
requirements.

## Traceability Model

Risk

↓

Security Objective

↓

Security Control

↓

Framework Reference

↓

Architecture Requirement

↓

Implementation Activity

## Framework Alignment

The mapping aligns control selection with:

-   NIST Cybersecurity Framework 2.0 concepts
-   ISO/IEC 27001:2022 control themes
-   Critical Infrastructure security practices

The mapping provides assessment traceability and does not represent
certification.

------------------------------------------------------------------------

# Document Status

Current Phase:

06 Security Control Mapping

Next Phase:

07 Target Security Architecture
