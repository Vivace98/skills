---
name: paper-matrix-extract
description: Extract structured information from an academic research paper and generate a literature matrix entry for Excel. Designed for demography, migration, and social science literature screening.
---

# Paper Matrix Extract

This skill extracts key structural information from an academic paper and formats it as a literature matrix entry for Excel.

Purpose: rapid literature screening.

---

# Strict Output Rules

Output must be contained in exactly ONE code block only.

Inside the code block, output exactly TWO lines only:

Line 1 = column names  
Line 2 = extracted values

Outside the code block, output nothing.

Use raw TSV (Tab-Separated Values).

Use literal TAB characters between columns.

Do NOT use spaces to simulate columns.

Do NOT align text manually.

Every column must contain exactly one value.

If information is missing, write:
none

Do NOT skip columns.

The number of values in Line 2 must exactly equal the number of columns in Line 1.

Do not use line breaks inside cells.

If multiple items belong in one cell, separate them with semicolons.

Do not add bullets, numbering, explanations, labels, or notes.

---

# Column Order (STRICT)

Paper  
Year  
Country/Region  
Data Source  
Data Type  
Sample / Unit  
Level of Analysis  
Gender Focus  
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

The output must exactly match this column order.

---

# Extraction Principles

Use short phrases only.

Avoid full sentences when possible.

Prefer compact keywords.

Focus on:

Introduction  
Literature Review  
Data  
Methods  
Results

---

# Level of Analysis Examples

Individual  
Household  
Regional  
Country

---

# Gender Focus Examples

Women  
Men  
Mixed

---

# Outcome Type Examples

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
Multinomial logit  
Linear probability model

---

# Identification Strategy Examples

IV  
Natural experiment  
Matching  
Panel fixed effects  
Sister fixed effects  
none

---

# Priority

High = core theory or key empirical study  
Medium = useful supporting literature  
Low = peripheral background literature

---

# Read Status

Default = Not read
