# AI Risk Assessment: CancerRisk-AI System
## DiagnosAI Sweden AB (Hypothetical)
### EU AI Act Article 9 Compliance

**Document version:** 1.0  
**Date:** June 2026  
**Author:** Saima Imran  
**Status:** Draft

---

## 1. SYSTEM OVERVIEW

| Field | Details |
|-------|---------|
| System name | CancerRisk-AI |
| Provider | DiagnosAI Sweden AB (hypothetical) |
| Intended purpose | Early cancer risk prediction for clinical decision support |
| Input data | Electronic health records, blood biomarkers, genomic markers |
| Output | Risk score (0-100) + classification (Low/Medium/High) + recommendations |
| End users | Clinical physicians in Swedish regional hospitals |
| Affected persons | Adult patients (18+) in Swedish healthcare system |
| Deployment context | Swedish regional healthcare |
| Risk classification | HIGH RISK — EU AI Act Annex III, Point 5(a) |

---

## 2. EU AI ACT ARTICLE 9 — RISK MANAGEMENT SYSTEM

Article 9 requires providers of high-risk AI systems to establish, implement, document and maintain a risk management system throughout the AI system's entire lifecycle.

### RISK 1: FALSE NEGATIVE PREDICTIONS
**Description:** AI system predicts LOW cancer risk for a patient who actually has cancer  
**Likelihood:** Medium  
**Severity:** CRITICAL — delayed diagnosis, patient harm  
**EU AI Act relevance:** Article 9, Article 15  

**Verifiable Criterion (VC-001):**
- Sensitivity must be at least 95% on validation dataset
- False negative rate must be below 5%
- Must be re-evaluated quarterly

**Mitigation measure:**
- Mandatory physician review for all medium/high risk scores
- System cannot autonomously classify without human confirmation

---

### RISK 2: ALGORITHMIC BIAS
**Description:** AI system performs differently across patient groups  
**Likelihood:** High  
**Severity:** HIGH — discriminatory outcomes  
**EU AI Act relevance:** Article 9, Article 10  

**Verifiable Criterion (VC-002):**
- Performance metrics must not differ by more than 5% across demographic groups
- Bias assessment must be documented before deployment

**Mitigation measure:**
- Training data must include representative samples from all demographic groups
- Separate performance evaluation per demographic group

---

### RISK 3: INSUFFICIENT EXPLANATION OF PREDICTIONS
**Description:** AI system provides risk score without adequate explanation  
**Likelihood:** High  
**Severity:** HIGH — unsafe clinical practice  
**EU AI Act relevance:** Article 13, Article 14  

**Verifiable Criterion (VC-003):**
- Every prediction must include top 5 contributing factors with percentage weights
- Explanation must be readable in under 30 seconds by clinical physician

**Mitigation measure:**
- SHAP values for every prediction
- Plain-language explanation alongside technical output

---

### RISK 4: PHYSICIAN OVER-RELIANCE ON AI
**Description:** Physician accepts AI recommendation without critical evaluation  
**Likelihood:** Medium  
**Severity:** HIGH — removes effective human oversight  
**EU AI Act relevance:** Article 14  

**Verifiable Criterion (VC-004):**
- System must require explicit physician confirmation before recommendation is logged
- Override rate must be monitored monthly

**Mitigation measure:**
- Mandatory confirmation step before accepting AI recommendation
- Monthly audit of physician override rates

---

### RISK 5: DATA PRIVACY BREACH
**Description:** Patient health data exposed  
**Likelihood:** Low  
**Severity:** CRITICAL — GDPR violation  
**EU AI Act relevance:** Article 9, Article 10  

**Verifiable Criterion (VC-005):**
- All patient data must be pseudonymised before use
- Access logs must be maintained

**Mitigation measure:**
- Pseudonymisation of all patient identifiers
- Role-based access control

---

### RISK 6: MODEL PERFORMANCE DEGRADATION
**Description:** AI model accuracy decreases over time  
**Likelihood:** High  
**Severity:** HIGH — inaccurate predictions  
**EU AI Act relevance:** Article 9, Article 15  

**Verifiable Criterion (VC-006):**
- Model performance must be monitored monthly
- Alert triggered if sensitivity drops more than 3% from baseline

**Mitigation measure:**
- Automated monthly performance dashboard
- Quarterly data drift analysis

---

### RISK 7: SYSTEM FAILURE / UNAVAILABILITY
**Description:** AI system becomes unavailable during clinical workflow  
**Likelihood:** Low  
**Severity:** Medium  
**EU AI Act relevance:** Article 15  

**Verifiable Criterion (VC-007):**
- System uptime must be at least 99.5% during clinical hours
- Fallback procedure must be documented and tested

**Mitigation measure:**
- Redundant system architecture
- Documented fallback to clinical judgment without AI

---

## 3. RISK SUMMARY TABLE

| Risk ID | Risk Description | Likelihood | Severity | Priority |
|---------|-----------------|-----------|---------|---------|
| RISK-001 | False negative predictions | Medium | Critical | HIGH |
| RISK-002 | Algorithmic bias | High | High | HIGH |
| RISK-003 | Insufficient explanation | High | High | HIGH |
| RISK-004 | Physician over-reliance | Medium | High | MEDIUM |
| RISK-005 | Data privacy breach | Low | Critical | HIGH |
| RISK-006 | Model performance drift | High | High | HIGH |
| RISK-007 | System unavailability | Low | Medium | LOW |

---

## 4. COMPLIANCE STATEMENT

This risk assessment was conducted in accordance with EU AI Act Article 9, Article 10, Article 15, ISO 42001, and GDPR.

**Assessment conducted by:** Saima Imran  
**Date:** June 2026  
**Next review date:** June 2027  

---

*DiagnosAI Sweden AB is a hypothetical company created for educational and research purposes.*
