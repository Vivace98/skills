---
name: paper-matrix-extract
description: Extract structured information from an academic research paper and generate one literature matrix row for Excel. Designed for demography, migration, and social science literature screening.
---

# Paper Matrix Extract

This skill extracts key structural information from an academic paper and formats it as **ONE literature matrix row**.

The purpose is **rapid literature screening**, not deep analysis.

Use this skill when the user:

- uploads a research paper
- pastes a paper abstract
- asks to extract literature information
- wants to fill a literature review matrix

The output should help the user quickly build a **literature database in Excel or Notion**.

---

# Extraction Principles

Focus on **core research structure**, not full summarization.

Prefer **short phrases**.

Do NOT generate long explanations.

If information is missing in the paper, write:

未明确说明

When extracting information, prioritize the following sections:

Introduction  
Literature Review  
Data  
Methods  
Results  

---

# Output Format

Always output **ONE single row only**.

Do not add explanations before or after the row.

Use **TSV format (Tab-Separated Values)** so the user can paste directly into Excel.

Column order must match exactly:

Paper  
Year  
Country/Region  
Data Source  
Sample / Unit  
Theory  
Research Question  
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

# Field Guidelines

Paper  
Author + year (e.g. Carling 2002)

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
Main question addressed by the study

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
Key empirical results (short phrases)

Contribution  
Main contribution claimed by the authors

Key Theory References  
Foundational theoretical literature cited

Closely Related Studies  
Empirical papers addressing a similar question

Research Gap  
Remaining unanswered questions

Priority  

High — core theory or key empirical study  
Medium — useful supporting literature  
Low — peripheral background literature

Read Status  

Default value: Not read
