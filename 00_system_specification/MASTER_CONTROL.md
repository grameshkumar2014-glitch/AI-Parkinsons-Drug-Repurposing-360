# AI Parkinson's Drug Repurposing 360
# MASTER CONTROL

**Project Version:** 0.1.0  
**Created:** 2026-10-03 04:08:20  
**Control Document Version:** 0.1.0  

---

## PURPOSE

This document is the central control file for the AI Parkinson's
Drug Repurposing 360 project.

No project phase may be marked COMPLETED until its required
deliverables and validation criteria have been satisfied.

No dependent phase should begin before its required dependencies
have been validated.

---

# STATUS DEFINITIONS

| Status | Meaning |
|---|---|
| NOT_STARTED | Work has not begun |
| IN_PROGRESS | Work is currently being executed |
| BLOCKED | Dependency or technical issue prevents progress |
| VALIDATION_REQUIRED | Work exists but validation is incomplete |
| COMPLETED | Deliverables and validation are complete |
| FAILED | Validation or execution failed |

---

# MASTER PHASE CONTROL

| ID | Phase | Dependencies | Validation | Status |
|---|---|---|---|---|
| P0 | Project Definition | None | Project charter and system specification validated | COMPLETED |
| P1 | Environment & Reproducibility | P0 | Environment health check passes | NOT_STARTED |
| P2 | Data Model | P0, P1 | Data schemas validated | NOT_STARTED |
| P3 | Candidate Library | P2 | Candidate ingestion and schema validation passes | NOT_STARTED |
| P4 | Evidence Ingestion | P2, P3 | Evidence records have provenance | NOT_STARTED |
| P5 | RAG Infrastructure | P4 | Retrieval test passes | NOT_STARTED |
| P6 | Parkinson's Ontology | P2, P4 | Ontology entities and relationships validated | NOT_STARTED |
| P7 | Knowledge Graph | P6 | Graph integrity checks pass | NOT_STARTED |
| P8 | Target Validation | P4, P6, P7 | Target evidence mapped and classified | NOT_STARTED |
| P9 | Mechanism Analysis | P8 | Mechanistic evidence profile generated | NOT_STARTED |
| P10 | Binding & Target Engagement | P8, P9 | Binding/engagement evidence classified | NOT_STARTED |
| P11 | Efficacy Analysis | P9, P10 | Preclinical and human efficacy evidence classified | NOT_STARTED |
| P12 | ADMET & Safety | P3, P4 | Safety and ADMET profile generated | NOT_STARTED |
| P13 | Biomarkers | P6, P8, P11 | Biomarker evidence mapped | NOT_STARTED |
| P14 | Patient Stratification | P13 | Candidate-to-patient subgroup relationships validated | NOT_STARTED |
| P15 | Clinical Intelligence | P4, P11, P12, P13 | Clinical trial evidence and outcomes mapped | NOT_STARTED |
| P16 | Failure Analysis | P11, P12, P15 | Negative and contradictory evidence captured | NOT_STARTED |
| P17 | Biology Deficit | P8, P9, P13, P14, P15, P16 | Uncertainty and biological gaps documented | NOT_STARTED |
| P18 | Information Gain | P17 | Information-gain framework validated | NOT_STARTED |
| P19 | Candidate Selection & Ranking | P10, P11, P12, P13, P14, P15, P16, P17, P18 | Ranking reproducibility test passes | NOT_STARTED |
| P20 | Validation | P19 | Independent validation checks pass | NOT_STARTED |
| P21 | Reports & GitHub Release | P20 | Final report and repository release validated | NOT_STARTED |

---

# COMPLETED CHECKPOINTS

## P0 — PROJECT DEFINITION

### P0.1 Project Structure
Status: COMPLETED

Evidence:
- 33 project directories created
- PROJECT_STRUCTURE_MANIFEST.txt created
- Directory validation passed

### P0.2 System Specification
Status: COMPLETED

Evidence:
- AI_PARKINSONS_DRUG_REPURPOSING_360_SYSTEM_SPECIFICATION.md
- SPECIFICATION_METADATA.txt
- File existence validation passed
- Non-empty validation passed

---

# CURRENT CONTROL POINT

Current completed phase:

**P0 — Project Definition**

Current next phase:

**P1 — Environment & Reproducibility**

No candidate analysis is authorized before the required
infrastructure phases are completed.

---

# SCIENTIFIC EXECUTION RULE

The following sequence must be preserved:

Project Definition
→ Environment
→ Data Model
→ Candidate Library
→ Evidence
→ RAG
→ Ontology
→ Knowledge Graph
→ Biological Evaluation
→ Clinical Evaluation
→ Failure Analysis
→ Biology Deficit
→ Information Gain
→ Ranking
→ Validation
→ Reporting

---

# ANTI-SKIPPING RULE

A later phase must not be marked COMPLETED when a required
dependency is:

- NOT_STARTED
- IN_PROGRESS
- BLOCKED
- VALIDATION_REQUIRED
- FAILED

Any dependency exception must be explicitly documented and
scientifically justified.

---

# DATA PROVENANCE RULE

Every important evidence record should retain:

- Source
- Source identifier
- Publication/trial identifier where applicable
- Retrieval date
- Evidence level
- Evidence type
- Candidate
- Target
- Disease context
- Study population
- Study design
- Outcome
- Direction of evidence
- Confidence
- Processing/version information

---

# NEGATIVE EVIDENCE RULE

Negative, null, contradictory, and failed evidence must be retained.

The system must not selectively remove evidence because it reduces
a candidate's ranking.

---

# AI TRACEABILITY RULE

AI-generated interpretations must be distinguishable from source
evidence.

Where possible, AI-generated claims must link to the underlying
evidence records.

---

# RANKING RULE

The final ranking must be reproducible from:

1. Defined input data
2. Evidence classification
3. Defined scoring methodology
4. Versioned code
5. Configuration
6. Model/version information

No manual alteration of the final ranking without an auditable
record.

---

# FINAL OUTPUT

The project will ultimately generate a research-prioritized
Parkinson's drug-repurposing shortlist.

The shortlist is a research output and is not a clinical treatment
recommendation.

---

# CHANGE CONTROL

Any change to:

- Scientific scope
- Evidence hierarchy
- Data schema
- Ranking methodology
- Candidate inclusion criteria
- Validation methodology

must be recorded in CHANGELOG.md.

---

# PROJECT VERSION

Current version: **0.1.0**

