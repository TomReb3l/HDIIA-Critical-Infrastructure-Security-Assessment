# HDIIA Critical Infrastructure Security Assessment

# Control Framework Matrix

Version: 1.0

Phase: 07 Security Control Mapping

------------------------------------------------------------------------

# Ελληνική Έκδοση

## 1. Σκοπός

Το Control Framework Matrix παρέχει λεπτομερή αντιστοίχιση μεταξύ:

-   αναγνωρισμένων risks
-   security controls
-   framework references
-   architecture components

Στόχος είναι η πλήρης traceability:

Risk → Control → Framework → Architecture

------------------------------------------------------------------------

# 2. Control Mapping Methodology

Η αξιολόγηση ακολουθεί:

Threat Scenario

↓

Risk

↓

Security Objective

↓

Security Control

↓

Framework Reference

↓

Architecture Component

------------------------------------------------------------------------

# 3. Control Framework Matrix

  --------------------------------------------------------------------------------------
  Risk         Security        Security       NIST CSF    ISO 27001       Architecture
  Reference    Control         Objective      Alignment   Alignment       Component
  ------------ --------------- -------------- ----------- --------------- --------------
  R-001        Endpoint        Protect        Protect /   Operations      Data
  Ransomware   Protection,     availability   Recover     Security,       Protection &
  Risk         Backup,         and recover                Business        Resilience
               Recovery        operations                 Continuity      Architecture
               Controls                                                   

  R-002        MFA, IAM, PAM   Protect        Protect     Access Control  Identity
  Credential                   identities and                             Security
  Compromise                   access                                     Architecture

  R-003        PAM, Access     Control        Protect /   Access Control, Identity
  Privileged   Review, Audit   privileged     Detect      Monitoring      Security
  Account      Logging         access                                     Architecture
  Misuse                                                                  

  R-004 Supply Third Party     Protect        Identify /  Supplier        Governance
  Chain        Risk Management external       Protect     Relationships   Architecture
  Compromise                   dependencies                               

  R-005        Segmentation,   Protect        Protect /   Network         Network
  Network      Firewall,       network        Detect      Security        Security
  Disruption   IDS/IPS         availability               Controls        Architecture
  --------------------------------------------------------------------------------------

------------------------------------------------------------------------

# 4. Security Control Categories

## Identity Controls

Controls:

-   Multi-Factor Authentication
-   Privileged Access Management
-   Role Based Access Control
-   Access Reviews

Purpose:

Μείωση κινδύνων μη εξουσιοδοτημένης πρόσβασης.

------------------------------------------------------------------------

## Network Controls

Controls:

-   Network Segmentation
-   Firewall Protection
-   IDS/IPS
-   Network Monitoring

Purpose:

Περιορισμός lateral movement.

------------------------------------------------------------------------

## Monitoring Controls

Controls:

-   Central Logging
-   SIEM
-   Detection Rules
-   Alert Management

Purpose:

Έγκαιρη ανίχνευση απειλών.

------------------------------------------------------------------------

## Resilience Controls

Controls:

-   Backup
-   Disaster Recovery
-   Recovery Testing

Purpose:

Διατήρηση κρίσιμων υπηρεσιών.

------------------------------------------------------------------------

# 5. Framework Alignment

## NIST Cybersecurity Framework

Mapping:

  Function   Purpose
  ---------- ------------------------------
  Identify   Asset and Risk Understanding
  Protect    Preventive Controls
  Detect     Security Monitoring
  Respond    Incident Management
  Recover    Service Restoration

------------------------------------------------------------------------

## ISO 27001 Alignment

Related control areas:

-   Access Control
-   Asset Management
-   Operations Security
-   Supplier Security
-   Incident Management
-   Business Continuity

------------------------------------------------------------------------

# 6. Architecture Traceability

Κάθε control συνδέεται με:

Risk

↓

Control

↓

Architecture Domain

↓

Implementation Requirement

------------------------------------------------------------------------

# English Version

## Purpose

The Control Framework Matrix maps identified risks to security controls,
standards and architecture components.

## Traceability Model

Risk → Control → Framework → Architecture

## Framework Alignment

The matrix aligns controls with:

-   NIST Cybersecurity Framework
-   ISO 27001 control areas
-   Critical infrastructure security practices

## Objective

Provide measurable traceability between cybersecurity risks and
implemented security capabilities.

------------------------------------------------------------------------

# Document Status

Current Phase:

07 Security Control Mapping

Artifact:

control_framework_matrix.md
