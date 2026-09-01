# HDIIA Critical Infrastructure Security Assessment

# Threat Model Methodology

Version: 1.0

Phase: 04 Threat Model

------------------------------------------------------------------------

# Ελληνική Έκδοση

# 1. Σκοπός Threat Modeling

Το Threat Modeling αποτελεί το επόμενο επίπεδο ανάλυσης μετά την
ολοκλήρωση:

-   Business Context
-   Critical Services
-   Asset Inventory
-   Asset Dependency Mapping

Στόχος είναι η συστηματική αναγνώριση πιθανών απειλών που μπορούν να
επηρεάσουν κρίσιμες υπηρεσίες, assets και εξαρτήσεις του οργανισμού.

Η διαδικασία υποστηρίζει:

-   αναγνώριση επιθετικών σεναρίων
-   αξιολόγηση έκθεσης
-   προετοιμασία Risk Assessment
-   επιλογή κατάλληλων security controls

------------------------------------------------------------------------

# 2. Μεθοδολογία

Η ανάλυση ακολουθεί το υφιστάμενο μοντέλο:

Business Context

↓

Critical Services

↓

Assets

↓

Dependencies

↓

Threats

↓

Risks

Η προσέγγιση είναι:

Business Driven → Asset Based → Risk Focused

Δεν εξετάζονται απειλές απομονωμένα, αλλά σε σχέση με:

-   επιχειρησιακή αξία
-   κρισιμότητα asset
-   dependency relationships
-   πιθανές επιπτώσεις

------------------------------------------------------------------------

# 3. Threat Categories

Οι απειλές κατηγοριοποιούνται σε:

## 3.1 Cyber Attacks

Περιλαμβάνονται:

-   Malware
-   Ransomware
-   Credential Theft
-   Exploitation of Vulnerabilities
-   Unauthorized Access

------------------------------------------------------------------------

## 3.2 Insider Threats

Περιλαμβάνονται:

-   Κακόβουλες ενέργειες προσωπικού
-   Λανθασμένες ενέργειες χρηστών
-   Κατάχρηση δικαιωμάτων πρόσβασης

------------------------------------------------------------------------

## 3.3 Infrastructure Threats

Περιλαμβάνονται:

-   Network failures
-   Hardware failures
-   Service disruption
-   Dependency failures

------------------------------------------------------------------------

## 3.4 External Threats

Περιλαμβάνονται:

-   Third-party compromise
-   Supply chain attacks
-   External service disruption

------------------------------------------------------------------------

# 4. Threat Actor Classification

Οι threat actors ταξινομούνται ως:

  Threat Actor                  Description
  ----------------------------- -----------------------------------------
  Nation State Actors           Advanced actors με στρατηγικούς στόχους
  Cyber Criminal Groups         Οικονομικά υποκινούμενες επιθέσεις
  Insider Users                 Εσωτερικοί χρήστες με πρόσβαση
  Contractors / Third Parties   Εξωτερικοί συνεργάτες
  Opportunistic Attackers       Αυτοματοποιημένες ή τυχαίες επιθέσεις

------------------------------------------------------------------------

# 5. Attack Surface Definition

Το Attack Surface περιλαμβάνει:

## External Surface

-   Internet exposed services
-   Remote access systems
-   External integrations

## Internal Surface

-   Network infrastructure
-   Identity systems
-   Applications
-   Data platforms

## Human Surface

-   Users
-   Administrators
-   Privileged accounts

------------------------------------------------------------------------

# 6. Threat Identification Process

Η διαδικασία:

1.  Επιλογή κρίσιμου asset

↓

2.  Ανάλυση dependencies

↓

3.  Αναγνώριση πιθανών threat actors

↓

4.  Καθορισμός threat scenario

↓

5.  Εκτίμηση πιθανής επίπτωσης

↓

6.  Μεταφορά στο Risk Assessment

------------------------------------------------------------------------

# 7. Risk Assessment Preparation

Το Threat Model θα παρέχει input για:

-   Likelihood assessment
-   Impact assessment
-   Risk scoring
-   Security control selection

Κάθε threat scenario θα συνδέεται με:

-   Asset
-   Business Service
-   Dependency
-   Threat Actor
-   Impact

------------------------------------------------------------------------

# 8. Framework Alignment

Η προσέγγιση ευθυγραμμίζεται με:

-   NIST Cybersecurity Framework
-   NIST Risk Management concepts
-   ISO 27001 security management principles
-   Critical Infrastructure security practices

------------------------------------------------------------------------

# English Version

# 1. Threat Modeling Purpose

Threat Modeling provides a structured approach to identify threats
affecting critical services, assets, and dependencies.

It supports:

-   attack scenario identification
-   exposure analysis
-   risk assessment preparation
-   security control selection

------------------------------------------------------------------------

# 2. Methodology

The analysis follows:

Business Context

↓

Critical Services

↓

Assets

↓

Dependencies

↓

Threats

↓

Risks

The approach is:

Business Driven → Asset Based → Risk Focused

------------------------------------------------------------------------

# 3. Threat Categories

Main categories:

-   Cyber Attacks
-   Insider Threats
-   Infrastructure Threats
-   External and Supply Chain Threats

------------------------------------------------------------------------

# 4. Threat Actor Classification

Threat actors include:

-   Nation State Actors
-   Cyber Criminal Groups
-   Insider Users
-   Contractors and Third Parties
-   Opportunistic Attackers

------------------------------------------------------------------------

# 5. Attack Surface Definition

Attack surface areas:

-   External exposure
-   Internal infrastructure
-   Human access points

------------------------------------------------------------------------

# 6. Threat Identification Process

Process:

Asset Selection

↓

Dependency Analysis

↓

Threat Actor Identification

↓

Scenario Creation

↓

Impact Evaluation

↓

Risk Assessment Input

------------------------------------------------------------------------

# 7. Risk Assessment Preparation

Threat scenarios will provide:

-   Asset context
-   Business impact
-   Likelihood information
-   Security control requirements

------------------------------------------------------------------------

# 8. Framework Alignment

Aligned with:

-   NIST Cybersecurity Framework
-   Risk Management principles
-   ISO 27001 security practices

------------------------------------------------------------------------

# Document Status

Current Phase:

04 Threat Model

Next Artifact:

Threat Scenario Register
