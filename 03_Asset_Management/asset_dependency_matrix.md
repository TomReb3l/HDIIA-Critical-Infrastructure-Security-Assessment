# HDIIA Critical Infrastructure Security Assessment

# Asset Dependency Matrix

## Έκδοση Ελληνική

## 1. Σκοπός

Το παρόν έγγραφο επεκτείνει το Asset Management Foundation και
καταγράφει τις σχέσεις εξάρτησης μεταξύ επιχειρησιακών υπηρεσιών, κύριων
assets και υποστηρικτικών τεχνικών υποδομών.

Στόχος είναι η αναγνώριση:

-   κρίσιμων εξαρτήσεων
-   σημείων αποτυχίας
-   επιπτώσεων διαθεσιμότητας
-   απαιτήσεων προστασίας

Η ανάλυση θα χρησιμοποιηθεί ως βάση για Threat Modeling και Risk
Assessment.

------------------------------------------------------------------------

# 2. Dependency Model

Η λογική εξάρτησης ακολουθεί:

Business Service

↓

Primary Asset

↓

Supporting Asset

↓

Technical Dependency

↓

Failure Impact

------------------------------------------------------------------------

# 3. Asset Relationship Model

Τα assets δεν αξιολογούνται μεμονωμένα.

Κάθε κρίσιμο asset εξετάζεται σε σχέση με:

-   επιχειρησιακή υπηρεσία που υποστηρίζει
-   άλλα assets από τα οποία εξαρτάται
-   εξωτερικές υπηρεσίες
-   πιθανές συνέπειες αστοχίας

------------------------------------------------------------------------

# 4. Business Service Dependencies

  -----------------------------------------------------------------------
  Business Service  Primary Asset     Supporting        Impact
                                      Dependency        
  ----------------- ----------------- ----------------- -----------------
  Identity and      Identity          Directory         Loss of user
  Access Management Infrastructure    Services, Network authentication
                                      Services          

  Critical          Application       Compute, Storage, Service
  Applications      Platforms         Database Services interruption

  Security          SOC Monitoring    SIEM, Log         Reduced detection
  Monitoring        Platform          Sources, Network  capability
                                      Visibility        

  Data Services     Data Platforms    Storage           Data availability
                                      Infrastructure,   impact
                                      Backup Systems    
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# 5. Technical Dependency Mapping

  -----------------------------------------------------------------------
  Asset             Dependency Type   Dependency        Security Impact
  ----------------- ----------------- ----------------- -----------------
  Identity          Direct            Network Core      Authentication
  Infrastructure                                        disruption

  Application       Direct            Compute           Application
  Platform                            Infrastructure    outage

  SIEM Platform     Direct            Log Collection    Monitoring
                                      Sources           degradation

  Data Platform     Direct            Storage Systems   Data availability
                                                        risk
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# 6. Single Points of Failure

Οι ακόλουθες κατηγορίες απαιτούν περαιτέρω αξιολόγηση:

-   Κεντρικές υπηρεσίες ταυτοποίησης
-   Core network infrastructure
-   Central monitoring platforms
-   Shared storage platforms

Τα συγκεκριμένα σημεία πρέπει να αξιολογηθούν σε επόμενη φάση Risk
Assessment.

------------------------------------------------------------------------

# 7. Security Impact

Το dependency mapping υποστηρίζει:

-   Availability analysis
-   Business continuity planning
-   Disaster recovery planning
-   Risk prioritization
-   Security control selection

------------------------------------------------------------------------

# English Version

# Purpose

This document extends the Asset Management Foundation by mapping
relationships between business services, primary assets, supporting
assets, and technical dependencies.

The objective is to identify:

-   critical dependencies
-   single points of failure
-   availability impacts
-   security protection requirements

------------------------------------------------------------------------

# Dependency Model

Business Service

↓

Primary Asset

↓

Supporting Asset

↓

Technical Dependency

↓

Failure Impact

------------------------------------------------------------------------

# Dependency Analysis Principles

Critical assets are analyzed together with their operational
dependencies.

Each dependency relationship considers:

-   supported business service
-   dependent assets
-   technical infrastructure
-   potential failure impact

------------------------------------------------------------------------

# Security Architecture Relevance

The dependency matrix provides the foundation for:

-   Threat Modeling
-   Risk Assessment
-   Security Control Mapping
-   Resilience Planning

------------------------------------------------------------------------

# Document Status

Phase:

Asset Management

Next Phase:

Threat Modeling Preparation
