# EU AI Act Compliance Framework for High-Risk Health AI Systems
## A Case Study: Cancer Risk Prediction AI (DiagnosAI Sweden AB)

**Author:** Saima Imran  
**GitHub:** github.com/saima-imran  
**Date:** June 2026  
**Status:** Work in Progress — Independent Research Project

---

## Project Overview

This repository presents a practical compliance framework applying the **EU AI Act (Regulation EU 2024/1689)** to a hypothetical high-risk health AI system. The framework translates high-level legal requirements into specific, verifiable, and testable software engineering criteria.

This project directly addresses the gap between:
- **WHAT** the EU AI Act requires (legal language)
- **HOW** software engineers can verify compliance (technical criteria)

This gap is analogous to how ISO 26262 required SOTIF and specific verification methods before it became practically implementable in automotive software engineering.

---

## Hypothetical Case Study: DiagnosAI Sweden AB

**Company:** DiagnosAI Sweden AB (hypothetical)  
**Product:** CancerRisk-AI — an AI system for early cancer risk prediction  
**Input data:** Patient electronic health records, blood biomarkers, genomic data  
**Output:** Cancer risk score (low/medium/high) + clinical recommendations  
**Users:** Clinical physicians in Swedish hospitals  
**Deployment:** Swedish regional healthcare systems  

### Why this AI system is HIGH RISK:
Under EU AI Act Annex III, Point 5(a): AI systems intended to be used for making decisions or assisting in making decisions related to the access to and enjoyment of essential private services including healthcare — are classified as HIGH RISK.

---

## Repository Structure

eu-ai-act-compliance-framework/
- README.md (you are here)
- 1_Risk_Assessment/cancer_ai_risk_assessment.md
- 3_Governance_Policy/ai_governance_policy.md

---

## Key EU AI Act Articles Covered

| Article | Requirement | Status |
|---------|-------------|--------|
| Article 9 | Risk Management System | Covered |
| Article 10 | Data Governance | Covered |
| Article 13 | Transparency | Covered |
| Article 14 | Human Oversight | Covered |
| Article 15 | Accuracy & Robustness | Covered |

---

## Research Motivation

The EU AI Act defines WHAT trustworthy AI must achieve. However, the software engineering community lacks standardised methods for HOW to verify these properties in practice. This project develops a prototype verification framework that:

1. Maps EU AI Act requirements to specific software engineering criteria
2. Defines pass/fail thresholds for each criterion  
3. Validates criteria against a realistic health AI scenario
4. Demonstrates the framework is domain-applicable

This work forms part of preparation for doctoral research in Trustworthy AI verification and EU AI Act compliance frameworks.

---

## Author Background

Saima Imran is a bioinformatician and computational data scientist with:
- M.Sc. in Bioinformatics (University of Skövde, Sweden)
- M.Sc. in Computer Science (UHR-assessed as Swedish Masterexamen)
- B.Sc. in Statistics and Computer Science
- Experience in clinical data harmonisation (SNOMED CT, ICD-10)
- 7 independent bioinformatics and health AI projects on GitHub
- Microsoft Azure AI Fundamentals (AI-900) certified

---

*This is an independent research and learning project. DiagnosAI Sweden AB is a hypothetical company created for educational purposes.*# eu-ai-act-compliance-framework
 EU AI Act compliance framework for high-risk health AI systems
