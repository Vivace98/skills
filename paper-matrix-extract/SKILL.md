---
name: paper-matrix-extract
description: Extract structured information from an academic research paper and generate a literature matrix entry for Excel. Designed for demography, migration, and social science literature screening.
---

# Paper Matrix Extract

This skill extracts key structural information from an academic paper and formats it as a **literature matrix entry for Excel**.

The purpose is **rapid literature screening**, not deep analysis.

Use this skill when the user:

- uploads a research paper
- pastes a paper abstract
- asks to extract literature information
- wants to fill a literature review matrix

The output helps the user build a **structured literature database**.

---

# Extraction Principles

Focus on **core research structure**.

Prefer **short phrases**.

Do NOT generate long explanations.

If information is missing in the paper, write:

none

When extracting information, prioritize:

Introduction  
Literature Review  
Data  
Methods  
Results  

---

# Output Format

Always output **exactly TWO lines only**.

Line 1 = column names  
Line 2 = extracted values

Use **TSV format (Tab-Separated Values)** so it can be pasted directly into Excel.

Do NOT add explanations before or after the two lines.

---

# Line 1 (Column Names)

Paper  
Year  
Country/Region  
Data Source  
Sample / Unit  
Theory  
Research Question  
Outcome Type  
DV  
Main IV  
Controls  
Mechanism  
Method Type  
Model Specification  
Identification Strategy  
Main Findings  
Contribution  
Key Theory References  
Closely Related Studies  
Research Gap  
Priority  
Read Status

---

# Line 2 (Extracted Information)

Extract corresponding information from the paper.

Rules:

• Use **short phrases**  
• If missing → **none**  
• Maintain exact column alignment

---

# Outcome Type Guidelines

Identify the **type of outcome studied**.

Examples:

Migration aspiration  
Migration intention  
Migration behavior  
Fertility  
Mortality  
Labor market outcome  
Education outcome

---

# Method Type Examples

Regression  
Event history analysis  
Multilevel model  
Qualitative analysis  
Mixed methods  

---

# Model Specification Examples

Logit  
Probit  
OLS  
Hazard model  
Fixed effects  
Random effects  

---

# Identification Strategy Examples

IV  
Natural experiment  
Matching  
Panel fixed effects  
none  

---

# Priority

High — core theory or key empirical study  
Medium — useful supporting literature  
Low — peripheral background literature  

---

# Read Status

Default value = Not read
