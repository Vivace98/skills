---
name: paper-matrix-extract
description: Extract structured information from an academic research paper and generate one literature matrix row for Excel. Designed for demography, migration, and social science literature screening.
---

# Paper Matrix Extract

This skill extracts key structural information from an academic paper and formats it as a **single literature matrix row**.

The purpose is **rapid literature screening**, not deep analysis.

Use this skill when the user:

- uploads a research paper
- pastes a paper abstract
- asks to extract literature information
- wants to fill a literature review matrix

The output should help the user quickly build a **literature database in Excel**.

---

# Extraction Principles

Focus on **core research structure**.

Do NOT generate long summaries.

Prefer **short phrases**.

If information is missing in the paper, write:

"未明确说明"

Whenever possible identify the section:

Introduction  
Literature Review  
Data  
Methods  
Results  

---

# Output Format

Always output **ONE table row**.

| Paper | Year | Country/Region | Data Source | Sample / Unit | Theory | Research Question | DV | Main IV | Controls | Mechanism | Method Type | Model Specification | Identification Strategy | Main Findings | Contribution | Key Theory References | Closely Related Studies | Research Gap | Priority | Read Status |

---

# Field Guidelines

Paper  
Author + year

Year  
Publication year

Country/Region  
Geographical focus of the study

Data Source  
Survey / census / register / panel / administrative data

Sample / Unit  
Individuals / households / regions etc.

Theory  
Conceptual or theoretical framework used

Research Question  
Main research question addressed by the paper

DV  
Dependent variable

Main IV  
Key explanatory variable

Controls  
Major control variables

Mechanism  
Mechanism variables tested (if any)

Method Type  
Regression / event history / multilevel / qualitative etc.

Model Specification  
Logit / OLS / hazard model / fixed effects / random effects etc.

Identification Strategy  
IV / natural experiment / matching / none etc.

Main Findings  
Key empirical results (short bullet style phrases)

Contribution  
Main contribution claimed by the authors

Key Theory References  
Foundational theoretical literature cited

Closely Related Studies  
Empirical papers addressing a similar question

Research Gap  
What the paper does not address or remaining questions

Priority  
Evaluate importance for deeper reading:

High — core theory or key empirical study  
Medium — useful supporting literature  
Low — peripheral background literature

Read Status  

Not read — only extracted  
Skimmed — quick scan  
Deep read — fully analyzed later
