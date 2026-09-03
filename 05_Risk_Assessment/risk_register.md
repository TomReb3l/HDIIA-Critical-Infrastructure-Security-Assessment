# HDIIA Critical Infrastructure Security Assessment

# Risk Register

**Version:** 1.1\
**Phase:** 05 Risk Assessment\
**Status:** Final Hardening --- 5×5 Risk Scoring Model

------------------------------------------------------------------------

# Ελληνική Έκδοση

## 1. Σκοπός

Το Risk Register αποτελεί το κύριο artifact της φάσης Risk Assessment.

Στόχος είναι η μετατροπή των threat scenarios σε αξιολογημένους
επιχειρησιακούς κινδύνους με συνεπή και επαναλήψιμη διαδικασία.

Βασίζεται στα:

-   Business Services Catalog
-   Asset Inventory Register
-   Asset Dependency Matrix
-   Threat Scenario Register
-   Risk Assessment Methodology

------------------------------------------------------------------------

## 2. Risk Register Model

Business Service\
↓\
Asset\
↓\
Dependency\
↓\
Threat Scenario\
↓\
Risk\
↓\
Control Treatment

Κάθε κίνδυνος συνδέεται με Business Service, Asset/Dependency, Threat
Scenario, Threat Actor, Owner, Controls και Treatment.

------------------------------------------------------------------------

## 3. Risk Scoring Model

**Risk Score = Likelihood Score × Impact Score**

  Risk Score   Severity
  ------------ ----------
  1--2         Low
  3--6         Moderate
  7--12        High
  13--25       Critical

------------------------------------------------------------------------

## 4. Risk Register

  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  Risk ID Threat       Asset ID        Affected Asset   Business Service Threat       Likelihood   Impact    Risk Severity   Risk Owner       Existing         Recommended
          Scenario ID                                                    Actor             Score    Score   Score                             Controls         Treatment
  ------- ------------ --------------- ---------------- ---------------- ---------- ------------ -------- ------- ---------- ---------------- ---------------- ---------------
  R-001   TS-001       HDIIA-APP-001   Application      Critical         Cyber                 3        4      12 High       Application      Endpoint         Improve
          Ransomware                   Platform         Applications     Criminal                                            Owner            Protection,      segmentation,
          Attack                                                         Group                                                                Backup Controls  recovery
                                                                                                                                                               testing,
                                                                                                                                                               ransomware
                                                                                                                                                               protection

  R-002   TS-002       HDIIA-IAM-001   Identity         Identity and     External              4        4      16 Critical   Identity Owner   Access Control,  Enforce MFA,
          Credential                   Infrastructure   Access           Threat                                                               Authentication   privileged
          Compromise                                    Management       Actor                                                                Policies         access
                                                                                                                                                               management

  R-003   TS-003       HDIIA-ADM-001   Administrative   Infrastructure   Insider               2        4       8 High       Security Manager Account          Strengthen
          Privileged                   Accounts         Operations       User                                                                 Monitoring       privileged
          Account                                                                                                                                              access
          Misuse                                                                                                                                               governance and
                                                                                                                                                               auditing

  R-004   TS-004       HDIIA-EXT-001   External         Critical         Third                 2        4       8 High       Vendor Owner     Supplier         Improve
          Supply Chain                 Dependencies     Services         Party                                                                Management       third-party
          Compromise                                                                                                                                           risk assessment

  R-005   TS-005       HDIIA-NET-001   Core Network     Infrastructure   Cyber                 3        3       9 High       Infrastructure   Network          Increase
          Network                      Services         Services         Actor /                                             Owner            Monitoring       resilience and
          Disruption                                                     Failure                                                                               redundancy
  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

------------------------------------------------------------------------

## 5. Risk Treatment Preparation

Τα αξιολογημένα risks χρησιμοποιούνται για:

-   Security Control Mapping
-   Risk Treatment Planning
-   Target Security Architecture
-   Security Improvement Roadmap

------------------------------------------------------------------------

# English Version

## Purpose

The Risk Register transforms identified threat scenarios into evaluated
business risks using a consistent 5×5 risk scoring model.

## Risk Scoring

**Risk Score = Likelihood Score × Impact Score**

## Risk Register Usage

The register provides traceability between:

Business Services → Assets → Threat Scenarios → Risks → Controls →
Treatments

The same scoring model is used by the Risk Register and Risk Heatmap.

------------------------------------------------------------------------

# Document Status

Current Phase:

05 Risk Assessment

Next Phase:

06 Security Control Mapping
