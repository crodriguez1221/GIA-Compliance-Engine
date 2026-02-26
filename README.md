\# Government Intelligence Agent (GIA)



\## Overview



The Government Intelligence Agent (GIA) is a graduate-level research prototype implementing a precedence-aware regulatory applicability engine for Washington State agencies.



The system models hierarchical legal authority, federal overlay activation, conflict detection, and explainable compliance reasoning using a hybrid symbolic-semantic architecture.



GIA integrates deterministic authority ranking with vector-based semantic retrieval to formalize regulatory applicability determination within bounded public-sector governance environments.



---



\## Research Motivation



Public-sector agencies operate within complex, multi-layered regulatory ecosystems composed of:



\- Federal statutes (e.g., HIPAA)

\- State statutes (RCW)

\- Administrative codes (WAC)

\- Agency-level policy standards (WaTech)



Determining which authority governs in multi-authority scenarios often requires manual legal interpretation, cross-referencing, and institutional knowledge.



GIA investigates whether regulatory hierarchy and precedence relationships can be partially formalized into a structured, explainable reasoning framework supported by a working prototype.



---



\## Core Contributions



\- Explicit modeling of constitutional authority hierarchy

\- Federal overlay logic (HIPAA preemption modeling)

\- Deterministic precedence ranking engine

\- Structured conflict detection framework

\- Semantic retrieval using vector embeddings

\- Explainable applicability output schema

\- Reproducible decision-support workflow



---



\## System Architecture



The prototype follows a layered hybrid architecture:



\*\*Presentation Layer\*\*

\- Streamlit interface for Agency Profile submission



\*\*Application Layer\*\*

\- FastAPI orchestration

\- Workflow controller



\*\*Reasoning Layer\*\*

\- Vector embedding similarity retrieval

\- Deterministic precedence ranking model

\- Conflict detection logic



\*\*Data Layer\*\*

\- Regulatory corpus storage

\- Vector index (FAISS)

\- Structured output logging



---



\## Methodology



The system implements a hybrid approach combining:



1\. Transformer-based sentence embeddings for contextual regulatory retrieval

2\. Cosine similarity-based vector matching

3\. Deterministic hierarchy scoring

4\. Conditional federal overlay activation

5\. Structured justification generation



This architecture separates semantic similarity from normative authority ordering to preserve constitutional hierarchy integrity.



---



\## Current Status



Initial repository scaffold and system architecture design complete.



Upcoming implementation phases:



\- Backend service development

\- Regulatory corpus segmentation

\- Embedding index construction

\- Precedence model implementation

\- Conflict detection module

\- Prototype UI integration



---



\## Installation (Development Environment – Prototype Setup)



Clone the repository:



git clone https://github.com/crodriguez1221/GIA-Compliance-Engine.git

cd GIA-Compliance-Engine



Create a virtual environment:



python -m venv .venv

.venv\\Scripts\\activate



Install dependencies:



pip install -r requirements.txt

