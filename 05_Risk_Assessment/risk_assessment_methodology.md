# HDIIA Critical Infrastructure Security Assessment

# Risk Assessment Methodology

**Version:** 1.1  
**Phase:** 05 Risk Assessment  
**Status:** Final Hardening — 5×5 Risk Scoring Model

---

# Ελληνική Έκδοση

## 1. Σκοπός Risk Assessment

Το Risk Assessment μετατρέπει τα αναγνωρισμένα threat scenarios σε αξιολογημένους επιχειρησιακούς κινδύνους και παρέχει συνεπή βάση για risk prioritization, security control selection και treatment planning.

Η αξιολόγηση βασίζεται στα:

- Business Services Catalog
- Asset Inventory Register
- Asset Dependency Matrix
- Threat Model Methodology
- Threat Scenario Register

Κύριοι στόχοι:

- αξιολόγηση Likelihood,
- αξιολόγηση Impact,
- υπολογισμός Risk Score,
- κατάταξη Risk Severity,
- ιεράρχηση κινδύνων,
- προετοιμασία security controls και treatment actions.

---

## 2. Risk Assessment Model

Η μεθοδολογική ακολουθία είναι:

**Business Context → Critical Services → Assets → Dependencies → Threat Scenarios → Risks → Security Controls → Treatment**

Κάθε κίνδυνος πρέπει να μπορεί να συσχετιστεί με:

- Business Service,
- Asset ή Dependency,
- Threat Scenario,
- Threat Actor / Failure Source,
- Likelihood,
- Impact,
- Risk Score,
- Risk Severity,
- Risk Owner,
- Existing Controls,
- Recommended Treatment.

---

## 3. Risk Scoring Formula

Η αξιολόγηση χρησιμοποιεί αριθμητικό μοντέλο 5×5.

**Risk Score = Likelihood Score × Impact Score**

Όπου:

- Likelihood Score = 1 έως 5
- Impact Score = 1 έως 5
- Risk Score = 1 έως 25

Το Risk Score χρησιμοποιείται για συνεπή prioritization. Δεν αποτελεί στατιστική πρόβλεψη πιθανότητας συμβάντος, αλλά ordinal risk-ranking mechanism για τις ανάγκες του assessment.

---

## 4. Likelihood Scale

| Score | Level | Description |
|---:|---|---|
| 1 | Rare | Το threat scenario θεωρείται εξαιρετικά απίθανο υπό τις υφιστάμενες συνθήκες και controls. |
| 2 | Unlikely | Το scenario είναι δυνατό αλλά δεν αναμένεται να συμβεί συχνά ή χωρίς πρόσθετες προϋποθέσεις. |
| 3 | Possible | Το scenario μπορεί ρεαλιστικά να συμβεί στο εξεταζόμενο περιβάλλον. |
| 4 | Likely | Το scenario έχει αυξημένη πιθανότητα εκδήλωσης λόγω threat exposure, weaknesses ή υφιστάμενων συνθηκών. |
| 5 | Almost Certain | Το scenario αναμένεται να εκδηλωθεί ή να επαναλαμβάνεται εάν δεν εφαρμοστούν ουσιαστικά mitigating controls. |

---

## 5. Impact Scale

| Score | Level | Description |
|---:|---|---|
| 1 | Insignificant | Ελάχιστη επίπτωση χωρίς ουσιαστική διακοπή κρίσιμων υπηρεσιών. |
| 2 | Minor | Περιορισμένη λειτουργική ή τεχνική επίπτωση με εύκολη αποκατάσταση. |
| 3 | Moderate | Αξιοσημείωτη επίπτωση σε υπηρεσίες, λειτουργίες ή security posture, με ανάγκη συντονισμένης αποκατάστασης. |
| 4 | Major | Σοβαρή επίπτωση σε κρίσιμες επιχειρησιακές λειτουργίες, διαθεσιμότητα, εμπιστευτικότητα ή ακεραιότητα. |
| 5 | Catastrophic | Εκτεταμένη ή παρατεταμένη επίπτωση σε κρίσιμες λειτουργίες, σημαντική επιχειρησιακή διακοπή ή σοβαρές συνέπειες για τον οργανισμό. |

---

## 6. Risk Severity Thresholds

| Risk Score | Severity | Treatment Priority |
|---:|---|---|
| 1–2 | Low | Accept / monitor according to risk owner judgment |
| 3–6 | Moderate | Monitor and treat where cost-effective or operationally justified |
| 7–12 | High | Treatment plan required or formally documented risk acceptance |
| 13–25 | Critical | Priority treatment required; acceptance requires explicit risk-owner authorization and escalation |

Η severity classification προκύπτει από το **numeric Risk Score**. Το numeric score είναι το authoritative value για την κατάταξη του risk.

---

## 7. 5×5 Risk Matrix

| Impact \ Likelihood | 1 Rare | 2 Unlikely | 3 Possible | 4 Likely | 5 Almost Certain |
|---|---:|---:|---:|---:|---:|
| **5 Catastrophic** | 5 Moderate | 10 High | 15 Critical | 20 Critical | 25 Critical |
| **4 Major** | 4 Moderate | 8 High | 12 High | 16 Critical | 20 Critical |
| **3 Moderate** | 3 Moderate | 6 Moderate | 9 High | 12 High | 15 Critical |
| **2 Minor** | 2 Low | 4 Moderate | 6 Moderate | 8 High | 10 High |
| **1 Insignificant** | 1 Low | 2 Low | 3 Moderate | 4 Moderate | 5 Moderate |

---

## 8. Risk Rating Procedure

Για κάθε threat scenario εφαρμόζονται τα παρακάτω βήματα:

1. Identify the relevant Business Service.
2. Identify the affected Asset or Dependency.
3. Confirm the Threat Scenario and threat source.
4. Assign a Likelihood Score (1–5).
5. Assign an Impact Score (1–5).
6. Calculate the Risk Score.
7. Derive Risk Severity from the defined thresholds.
8. Identify the Risk Owner.
9. Record Existing Controls.
10. Define Recommended Treatment.
11. Feed prioritized risks into Security Control Mapping and the Security Improvement Roadmap.

---

## 9. Risk Acceptance and Treatment Criteria

- **Critical risks (13–25):** απαιτούν priority treatment. Η αποδοχή τους πρέπει να είναι ρητά τεκμηριωμένη και εγκεκριμένη από τον αρμόδιο Risk Owner.
- **High risks (7–12):** απαιτούν treatment plan ή τεκμηριωμένη risk acceptance.
- **Moderate risks (3–6):** παρακολουθούνται και αντιμετωπίζονται βάσει business priority, exposure και treatment cost.
- **Low risks (1–2):** μπορούν να γίνουν αποδεκτοί ή να παρακολουθούνται, εφόσον δεν υπάρχουν πρόσθετοι business ή regulatory drivers.

Risk acceptance δεν σημαίνει ότι ο κίνδυνος εξαλείφθηκε. Σημαίνει ότι ο residual exposure γίνεται συνειδητά αποδεκτός από τον αρμόδιο owner.

---

## 10. Scoring Governance

Για να διατηρείται consistency μεταξύ Risk Register, Risk Heatmap και downstream artifacts:

- κάθε risk πρέπει να καταγράφει explicit Likelihood Score και Impact Score,
- το Risk Score πρέπει να υπολογίζεται με τον ίδιο τύπο,
- το Risk Severity πρέπει να προκύπτει μόνο από τα καθορισμένα thresholds,
- qualitative labels δεν πρέπει να υπερισχύουν του numeric score,
- κάθε αλλαγή σε Likelihood ή Impact πρέπει να οδηγεί σε επανυπολογισμό του Risk Score,
- το Risk Heatmap πρέπει να απεικονίζει τις ίδιες numeric coordinates με το Risk Register.

---

## 11. Framework Alignment

Η μεθοδολογία ευθυγραμμίζεται σε επίπεδο risk-management principles με:

- NIST risk management concepts,
- NIST Cybersecurity Framework,
- ISO/IEC 27001 risk-based security principles.

Η συγκεκριμένη 5×5 μήτρα αποτελεί project-level risk prioritization model για το HDIIA assessment και δεν παρουσιάζεται ως επίσημη αριθμητική μήτρα κάποιου από τα παραπάνω frameworks.

---

# English Version

## 1. Risk Assessment Purpose

The Risk Assessment converts identified threat scenarios into evaluated business risks and provides a consistent basis for risk prioritization, security control selection, and treatment planning.

It is based on:

- Business Services Catalog
- Asset Inventory Register
- Asset Dependency Matrix
- Threat Model Methodology
- Threat Scenario Register

Primary objectives are to:

- evaluate Likelihood,
- evaluate Impact,
- calculate Risk Score,
- classify Risk Severity,
- prioritize risks,
- prepare security controls and treatment actions.

---

## 2. Risk Assessment Model

The assessment follows:

**Business Context → Critical Services → Assets → Dependencies → Threat Scenarios → Risks → Security Controls → Treatment**

Each risk should be traceable to:

- Business Service,
- Asset or Dependency,
- Threat Scenario,
- Threat Actor / Failure Source,
- Likelihood,
- Impact,
- Risk Score,
- Risk Severity,
- Risk Owner,
- Existing Controls,
- Recommended Treatment.

---

## 3. Risk Scoring Formula

The assessment uses a 5×5 numerical model.

**Risk Score = Likelihood Score × Impact Score**

Where:

- Likelihood Score = 1 to 5
- Impact Score = 1 to 5
- Risk Score = 1 to 25

The score is used for consistent prioritization. It is not a statistical forecast of event probability; it is an ordinal risk-ranking mechanism for this assessment.

---

## 4. Likelihood Scale

| Score | Level | Description |
|---:|---|---|
| 1 | Rare | The threat scenario is considered highly unlikely under current conditions and controls. |
| 2 | Unlikely | The scenario is possible but is not expected to occur frequently or without additional preconditions. |
| 3 | Possible | The scenario can realistically occur within the assessed environment. |
| 4 | Likely | The scenario has elevated likelihood because of threat exposure, weaknesses, or current operating conditions. |
| 5 | Almost Certain | The scenario is expected to occur or recur if meaningful mitigating controls are not implemented. |

---

## 5. Impact Scale

| Score | Level | Description |
|---:|---|---|
| 1 | Insignificant | Minimal impact with no material disruption to critical services. |
| 2 | Minor | Limited operational or technical impact with straightforward recovery. |
| 3 | Moderate | Noticeable impact to services, operations, or security posture requiring coordinated recovery. |
| 4 | Major | Serious impact to critical business operations, availability, confidentiality, or integrity. |
| 5 | Catastrophic | Extensive or prolonged impact to critical operations, major business disruption, or severe organizational consequences. |

---

## 6. Risk Severity Thresholds

| Risk Score | Severity | Treatment Priority |
|---:|---|---|
| 1–2 | Low | Accept / monitor according to risk owner judgment |
| 3–6 | Moderate | Monitor and treat where cost-effective or operationally justified |
| 7–12 | High | Treatment plan required or formally documented risk acceptance |
| 13–25 | Critical | Priority treatment required; acceptance requires explicit risk-owner authorization and escalation |

Risk Severity is derived from the **numeric Risk Score**, which is the authoritative value for risk classification.

---

## 7. 5×5 Risk Matrix

| Impact \ Likelihood | 1 Rare | 2 Unlikely | 3 Possible | 4 Likely | 5 Almost Certain |
|---|---:|---:|---:|---:|---:|
| **5 Catastrophic** | 5 Moderate | 10 High | 15 Critical | 20 Critical | 25 Critical |
| **4 Major** | 4 Moderate | 8 High | 12 High | 16 Critical | 20 Critical |
| **3 Moderate** | 3 Moderate | 6 Moderate | 9 High | 12 High | 15 Critical |
| **2 Minor** | 2 Low | 4 Moderate | 6 Moderate | 8 High | 10 High |
| **1 Insignificant** | 1 Low | 2 Low | 3 Moderate | 4 Moderate | 5 Moderate |

---

## 8. Risk Rating Procedure

For each threat scenario:

1. Identify the relevant Business Service.
2. Identify the affected Asset or Dependency.
3. Confirm the Threat Scenario and threat source.
4. Assign a Likelihood Score (1–5).
5. Assign an Impact Score (1–5).
6. Calculate the Risk Score.
7. Derive Risk Severity from the defined thresholds.
8. Identify the Risk Owner.
9. Record Existing Controls.
10. Define Recommended Treatment.
11. Feed prioritized risks into Security Control Mapping and the Security Improvement Roadmap.

---

## 9. Risk Acceptance and Treatment Criteria

- **Critical risks (13–25):** require priority treatment. Acceptance must be explicitly documented and approved by the accountable Risk Owner.
- **High risks (7–12):** require a treatment plan or documented risk acceptance.
- **Moderate risks (3–6):** should be monitored and treated according to business priority, exposure, and treatment cost.
- **Low risks (1–2):** may be accepted or monitored where no additional business or regulatory driver requires treatment.

Risk acceptance does not mean the risk has been eliminated. It means that the residual exposure is consciously accepted by the accountable owner.

---

## 10. Scoring Governance

To maintain consistency between the Risk Register, Risk Heatmap, and downstream artifacts:

- every risk must record explicit Likelihood and Impact scores,
- Risk Score must use the same calculation formula,
- Risk Severity must be derived only from the defined thresholds,
- qualitative labels must not override the numeric score,
- changes to Likelihood or Impact require Risk Score recalculation,
- the Risk Heatmap must use the same numeric coordinates recorded in the Risk Register.

---

## 11. Framework Alignment

The methodology aligns at the risk-management-principles level with:

- NIST risk management concepts,
- NIST Cybersecurity Framework,
- ISO/IEC 27001 risk-based security principles.

The 5×5 matrix is a project-level risk prioritization model developed for the HDIIA assessment and is not presented as an official numerical matrix mandated by those frameworks.

---

# Document Status

**Current Phase:** 05 Risk Assessment  
**Next Artifact:** Risk Register  
**Methodology Status:** 5×5 scoring model aligned with the HDIIA Risk Heatmap
