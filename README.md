# Government Intelligence Agent (GIA)

## Research Prototype: Regulatory Applicability & Conflict Resolution Engine

The Government Intelligence Agent (GIA) is a graduate-level research prototype designed to model regulatory hierarchy, strictness-based conflict resolution, and citation-grounded compliance decision support for Washington State agencies.

The system formalizes legal precedence and privacy/security strictness principles into explicit computational functions and evaluates their effectiveness using measurable performance metrics.

---

## For Security & Compliance Professionals (Quick Overview)

GIA implements:

- Deterministic authority ranking (federal > state > regulation > policy)
- Strictness-based conflict resolution modeling
- Citation-grounded output generation
- Structured audit trace logging
- Evaluation against gold-standard compliance scenarios

The prototype demonstrates how regulatory hierarchy can be encoded into transparent, reproducible computational workflows rather than relying on opaque AI inference.

---

## Research Objective

The core research question:

> Can regulatory hierarchy and strictness-based conflict resolution be encoded as computational constraints and evaluated for accuracy within a bounded authority corpus?

The system investigates whether a hybrid rule-based and retrieval-grounded architecture can:

- Identify applicable authorities for structured agency scenarios
- Detect and classify regulatory conflicts
- Apply precedence and strictness models deterministically
- Produce citation-backed compliance guidance
- Achieve measurable precision and recall against a gold-standard dataset

---

## Authority Corpus (Bounded MVP)

### Federal
- HIPAA Privacy Rule

### Washington State
- RCW 42.56 – Public Records Act
- RCW 19.255 – Data Breach Notification
- RCW 70.02 – Uniform Health Care Information Act

### Regulation
- Relevant WAC sections tied to above RCWs

### Policy
- WaTech Data Classification Standard
- WaTech IT Security Standard

The corpus is intentionally bounded to preserve experimental control, modeling clarity, and reproducibility.

---

## System Architecture

The GIA system implements a layered architecture:

1. Structured Scenario Input Layer  
2. Metadata-Driven Applicability Filter  
3. Precedence & Strictness Conflict Model  
4. Retrieval Engine (Vector Index – FAISS planned)  
5. Citation-Grounded Output Layer  

### Data Layer
- SQLite (local relational storage for MVP)
- Structured run logging for reproducibility
- Version-controlled authority corpus

---

## Modeling Formulation

Two core decision functions are implemented:

**Direct Conflict Resolution:**

argmax P(a)

**Additive Constraint Resolution:**

argmax S(a)

Where:

- P(a) = Precedence rank of authority *a*
- S(a) = Strictness score of authority *a*

These functions operationalize legal hierarchy and privacy/security dominance principles into deterministic computational constraints.

---

## Technology Stack (MVP)

- Python 3.11
- FastAPI (backend – planned integration)
- Streamlit (prototype UI)
- SQLite (local database)
- FAISS (vector retrieval – experimental component)
- GitHub (version control)

---

## Installation (Development Environment)

```bash
git clone https://github.com/crodriguez1221/GIA-Compliance-Engine.git
cd GIA-Compliance-Engine
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt