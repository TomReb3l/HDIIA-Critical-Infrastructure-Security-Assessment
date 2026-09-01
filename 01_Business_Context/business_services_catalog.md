# HDIIA Business Services Catalog


# Ελληνική Έκδοση


## 1. Σκοπός Εγγράφου

Το παρόν έγγραφο καθορίζει και περιγράφει τις κρίσιμες επιχειρησιακές υπηρεσίες (Critical Business Services) που παρέχονται από τη Hellenic Defense Information Infrastructure Agency (HDIIA).

Στόχος είναι η κατανόηση:

- Των υπηρεσιών που πρέπει να προστατευθούν
- Της επιχειρησιακής τους αξίας
- Των τεχνικών και λειτουργικών εξαρτήσεων
- Των απαιτήσεων διαθεσιμότητας και ασφάλειας

Το Business Services Catalog αποτελεί βάση για τα επόμενα στάδια:

- Asset Identification
- Asset Criticality Classification
- Threat Modeling
- Risk Assessment
- Security Architecture Design


---

# 2. Critical Services Overview


Η HDIIA παρέχει κρίσιμες υπηρεσίες πληροφοριακής υποδομής οι οποίες υποστηρίζουν τη λειτουργία κυβερνητικών οργανισμών και απαιτούν αυξημένα επίπεδα προστασίας.


Οι βασικές κρίσιμες υπηρεσίες περιλαμβάνουν:


## 2.1 Secure Data Storage Service

Υπηρεσία ασφαλούς αποθήκευσης και διαχείρισης ευαίσθητων πληροφοριών.

Η υπηρεσία υποστηρίζει:

- Αποθήκευση κυβερνητικών δεδομένων
- Διατήρηση ακεραιότητας δεδομένων
- Ελεγχόμενη πρόσβαση σε πληροφορίες


Κρίσιμες απαιτήσεις:

- Confidentiality
- Integrity
- Availability


---

## 2.2 Secure Information Exchange Service

Υπηρεσία ασφαλούς ανταλλαγής πληροφοριών μεταξύ εξουσιοδοτημένων κυβερνητικών φορέων.

Υποστηρίζει:

- Ασφαλή διαμοιρασμό δεδομένων
- Ελεγχόμενη επικοινωνία
- Προστασία μεταφερόμενων πληροφοριών


---

## 2.3 Identity and Access Management Service

Υπηρεσία διαχείρισης ψηφιακών ταυτοτήτων και δικαιωμάτων πρόσβασης.

Περιλαμβάνει:

- User Identity Management
- Authentication Services
- Authorization Controls
- Privileged Access Management


Η υπηρεσία αποτελεί κρίσιμο σημείο ελέγχου επειδή παραβίασή της μπορεί να οδηγήσει σε:

- Unauthorized Access
- Privilege Escalation
- Lateral Movement


---

## 2.4 Critical Application Hosting Service

Υπηρεσία φιλοξενίας εφαρμογών που υποστηρίζουν κρίσιμες κυβερνητικές λειτουργίες.

Περιλαμβάνει:

- Application Platforms
- Server Infrastructure
- Supporting Services


---

## 2.5 Security Monitoring Service

Υπηρεσία παρακολούθησης ασφάλειας και ανίχνευσης συμβάντων.

Περιλαμβάνει:

- Log Collection
- Security Monitoring
- Alert Generation
- Incident Detection


---

## 2.6 Data Center Infrastructure Service

Υπηρεσία παροχής φυσικής και τεχνικής υποδομής για τη λειτουργία κρίσιμων συστημάτων.

Περιλαμβάνει:

- Server Facilities
- Network Infrastructure
- Environmental Monitoring
- Physical Security Systems


---

# 3. Service Classification


Οι υπηρεσίες ταξινομούνται σύμφωνα με την επιχειρησιακή τους κρισιμότητα.


## Criticality Levels


## Level 1 — Mission Critical

Υπηρεσίες των οποίων η διακοπή μπορεί να προκαλέσει σημαντική επιχειρησιακή επίπτωση.

Παραδείγματα:

- Identity Services
- Data Storage Services
- Security Monitoring


---

## Level 2 — Business Critical

Υπηρεσίες σημαντικές για τη λειτουργία του οργανισμού αλλά με δυνατότητα περιορισμένης προσωρινής διακοπής.

Παραδείγματα:

- Application Hosting Services
- Information Exchange Services


---

## Level 3 — Supporting Services

Υπηρεσίες που υποστηρίζουν τη λειτουργία χωρίς άμεση επίπτωση στη βασική αποστολή.


---

# 4. Service Criticality Criteria


Η κρισιμότητα κάθε υπηρεσίας αξιολογείται βάσει:


## Business Impact

Εξετάζεται:

- Επιχειρησιακή επίπτωση από διακοπή
- Επίπτωση σε κυβερνητικές λειτουργίες
- Επίπτωση σε χρήστες και συνεργαζόμενους φορείς


## CIA Impact

Αξιολογούνται:

### Confidentiality

Επίπτωση από μη εξουσιοδοτημένη αποκάλυψη δεδομένων.


### Integrity

Επίπτωση από αλλοίωση ή μη εξουσιοδοτημένη τροποποίηση δεδομένων.


### Availability

Επίπτωση από μη διαθεσιμότητα υπηρεσίας.


## Dependency Criticality

Εξετάζονται οι εξαρτήσεις κάθε υπηρεσίας από:

- Άλλα συστήματα
- Υποδομές
- Ανθρώπινο δυναμικό
- Εξωτερικούς παρόχους


---

# 5. Business Dependencies


Οι κρίσιμες υπηρεσίες εξαρτώνται από:


## Organizational Dependencies

- Security Operations Teams
- Infrastructure Teams
- Facility Management
- Service Owners


## Process Dependencies

- Incident Response Processes
- Change Management
- Access Management
- Business Continuity Procedures


---

# 6. Technical Dependencies


Οι υπηρεσίες βασίζονται σε:


## Infrastructure Dependencies

- Servers
- Storage Systems
- Network Infrastructure
- Data Center Facilities


## Identity Dependencies

- Directory Services
- Authentication Systems
- Access Control Mechanisms


## Security Dependencies

- Firewalls
- Logging Systems
- SIEM Platforms
- Endpoint Security Controls


## Environmental Dependencies

- Power Systems
- Cooling Systems
- Physical Access Systems


---

# 7. Availability Requirements


Λόγω του κρίσιμου χαρακτήρα των υπηρεσιών, απαιτούνται:


## High Availability

Οι υπηρεσίες πρέπει να παρέχουν:

- Συνεχή λειτουργία
- Μειωμένο downtime
- Ανθεκτικότητα σε αστοχίες


## Operational Resilience

Απαιτούνται:

- Backup Procedures
- Recovery Capabilities
- Incident Response Readiness


## Service Continuity

Η διαθεσιμότητα πρέπει να προστατεύεται από:

- Cyber Incidents
- Physical Incidents
- Infrastructure Failures


---

# 8. Security Requirements per Service


## Secure Data Storage

Απαιτήσεις:

- Encryption
- Access Control
- Data Integrity Protection
- Backup Protection


## Information Exchange

Απαιτήσεις:

- Secure Communication
- Authentication
- Data Protection Controls


## Identity Services

Απαιτήσεις:

- Strong Authentication
- Least Privilege
- Privileged Access Protection
- Monitoring


## Application Hosting

Απαιτήσεις:

- Secure Configuration
- Patch Management
- Network Segmentation


## Security Monitoring

Απαιτήσεις:

- Centralized Logging
- Alerting
- Incident Detection Capability


## Data Center Infrastructure

Απαιτήσεις:

- Physical Access Control
- CCTV Monitoring
- Environmental Protection
- Cyber-Physical Security Controls


---

# 9. Business Impact Considerations


Η αποτυχία μιας κρίσιμης υπηρεσίας μπορεί να οδηγήσει σε:


## Operational Impact

- Διακοπή κυβερνητικών υπηρεσιών
- Μείωση επιχειρησιακής αποτελεσματικότητας
- Καθυστέρηση κρίσιμων διαδικασιών


## Security Impact

- Unauthorized Access
- Data Exposure
- Loss of System Control


## Financial and Reputation Impact

- Μείωση εμπιστοσύνης
- Αυξημένο κόστος αποκατάστασης
- Επιχειρησιακές συνέπειες


---

# 10. Interview Justification Points


## Question:

Why create a business services catalog before asset inventory?


## Answer:

Because assets only have meaning when they are connected to the business services they support. Service criticality determines asset priority.


---

## Question:

How do you determine which services are most important?


## Answer:

By evaluating business impact, CIA requirements, dependencies and operational importance.


---

## Question:

Why include physical infrastructure dependencies?


## Answer:

Critical services depend on both cyber and physical components. A failure in power, cooling or physical access can directly affect digital availability.


---

# English Version


## 1. Document Purpose

This document defines the critical business services provided by the Hellenic Defense Information Infrastructure Agency (HDIIA).

The objective is to understand:

- Services requiring protection
- Business value
- Technical and operational dependencies
- Availability and security requirements


The Business Services Catalog supports:

- Asset Identification
- Asset Criticality Classification
- Threat Modeling
- Risk Assessment
- Security Architecture Design


---

# 2. Critical Services Overview


HDIIA provides critical information infrastructure services supporting government organizations.


The main services include:


## 2.1 Secure Data Storage Service

Secure storage and management of sensitive information.

Supports:

- Government data storage
- Data integrity protection
- Controlled information access


---

## 2.2 Secure Information Exchange Service

Secure exchange of information between authorized government entities.

Supports:

- Secure data sharing
- Controlled communication
- Information protection


---

## 2.3 Identity and Access Management Service

Management of digital identities and access permissions.

Includes:

- User Identity Management
- Authentication Services
- Authorization Controls
- Privileged Access Management


Compromise may result in:

- Unauthorized Access
- Privilege Escalation
- Lateral Movement


---

## 2.4 Critical Application Hosting Service

Hosting of applications supporting critical government operations.


Includes:

- Application Platforms
- Server Infrastructure
- Supporting Services


---

## 2.5 Security Monitoring Service

Security visibility and incident detection capabilities.

Includes:

- Log Collection
- Monitoring
- Alert Generation
- Incident Detection


---

## 2.6 Data Center Infrastructure Service

Physical and technical infrastructure supporting critical systems.

Includes:

- Server Facilities
- Network Infrastructure
- Environmental Monitoring
- Physical Security Systems


---

# 3. Service Classification


Services are classified according to business criticality.


## Level 1 — Mission Critical

Services where disruption may create significant operational impact.


Examples:

- Identity Services
- Data Storage Services
- Security Monitoring


## Level 2 — Business Critical

Important services with limited tolerance for disruption.


Examples:

- Application Hosting
- Information Exchange


## Level 3 — Supporting Services

Services supporting organizational operations.


---

# 4. Service Criticality Criteria


Criticality is evaluated through:


## Business Impact

Including:

- Operational disruption
- Government service impact
- Stakeholder impact


## CIA Impact

Evaluating:

- Confidentiality
- Integrity
- Availability


## Dependency Criticality

Including dependencies on:

- Systems
- Infrastructure
- Personnel
- External providers


---

# 5. Business Dependencies


Services depend on:


- Security Operations Teams
- Infrastructure Teams
- Facility Management
- Service Owners


Processes include:

- Incident Response
- Change Management
- Access Management
- Business Continuity


---

# 6. Technical Dependencies


Services depend on:


## Infrastructure

- Servers
- Storage Systems
- Network Infrastructure
- Data Center Facilities


## Identity

- Directory Services
- Authentication Systems
- Access Controls


## Security

- Firewalls
- Logging Systems
- SIEM Platforms
- Endpoint Security Controls


## Environmental

- Power Systems
- Cooling Systems
- Physical Access Systems


---

# 7. Availability Requirements


Critical services require:


## High Availability

Including:

- Continuous operation
- Reduced downtime
- Fault tolerance


## Operational Resilience

Including:

- Backup Procedures
- Recovery Capabilities
- Incident Readiness


---

# 8. Security Requirements per Service


Requirements include:


## Data Storage

- Encryption
- Access Control
- Integrity Protection
- Backup Protection


## Information Exchange

- Secure Communication
- Authentication
- Data Protection


## Identity Services

- Strong Authentication
- Least Privilege
- Privileged Access Protection


## Application Hosting

- Secure Configuration
- Patch Management
- Network Segmentation


## Security Monitoring

- Centralized Logging
- Alerting
- Detection Capability


## Data Center Infrastructure

- Physical Access Control
- CCTV Monitoring
- Environmental Protection
- Cyber-Physical Security Controls


---

# 9. Business Impact Considerations


Service failure may result in:


## Operational Impact

- Government service disruption
- Reduced operational effectiveness
- Delayed critical processes


## Security Impact

- Unauthorized Access
- Data Exposure
- Loss of System Control


## Reputation Impact

- Reduced trust
- Increased recovery cost
- Business consequences


---

# 10. Interview Justification Points


## Question:

Why create a business services catalog before asset inventory?


## Answer:

Assets only have meaning when connected to the business services they support. Service criticality determines asset priority.


## Question:

How do you determine which services are most important?


## Answer:

By evaluating business impact, CIA requirements, dependencies and operational importance.


## Question:

Why include physical infrastructure dependencies?


## Answer:

Critical services depend on both cyber and physical components. Failures in power, cooling or physical access can directly affect digital availability.


