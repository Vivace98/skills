---
name: paper-matrix-extract
description: Extract structured information from an academic research paper and generate a literature matrix entry for Excel. Designed for demography, migration, and social science literature screening.
---

# Paper Matrix Extract

This skill extracts structured information from an academic paper and formats it as a literature matrix entry for Excel.

Purpose: rapid literature screening.

---

# Strict Output Rules

Output must be contained in exactly ONE code block only.

Inside the code block, output exactly TWO lines only.

Line 1 must be the header row.
Line 2 must be the value row.

Outside the code block, output nothing.

Use raw TSV only.

Use literal TAB characters between columns.

Do NOT use spaces to simulate columns.

Do NOT align text manually.

Do NOT add bullets, numbering, explanations, labels, notes, or blank lines.

Do NOT use line breaks inside cells.

If multiple items belong in one cell, separate them with semicolons.

Every column must contain exactly one value.

If information is missing, uncertain, not reported, or cannot be inferred directly from the paper, write:
none

Do NOT skip columns.

Do NOT merge columns.

Do NOT change column names.

Do NOT change column order.

The number of cells in Line 2 must exactly equal the number of header columns in Line 1.

---

# Header Row (MUST MATCH EXACTLY)

Line 1 must be exactly this header row, character-for-character, in TSV format:

Paper	Year	Country/Region	Data Source	Data Type	Sample / Unit	Level of Analysis	Gender Focus	Theory	Research Question	Outcome Type	DV	Main IV	Controls	Mechanism	Method Type	Model Specification	Identification Strategy	Main Findings	Contribution	Key Theory References	Closely Related Studies	Research Gap	Priority	Read Status

Never paraphrase, shorten, expand, reorder, or reformat this header.

---

# Value Row Rules

Line 2 must map one-to-one to the header row above.

That means:

Column 1 = Paper  
Column 2 = Year  
Column 3 = Country/Region  
Column 4 = Data Source  
Column 5 = Data Type  
Column 6 = Sample / Unit  
Column 7 = Level of Analysis  
Column 8 = Gender Focus  
Column 9 = Theory  
Column 10 = Research Question  
Column 11 = Outcome Type  
Column 12 = DV  
Column 13 = Main IV  
Column 14 = Controls  
Column 15 = Mechanism  
Column 16 = Method Type  
Column 17 = Model Specification  
Column 18 = Identification Strategy  
Column 19 = Main Findings  
Column 20 = Contribution  
Column 21 = Key Theory References  
Column 22 = Closely Related Studies  
Column 23 = Research Gap  
Column 24 = Priority  
Column 25 = Read Status

If a paper does not provide content for any column, write none in that cell.

Never leave a cell empty.

---

# Extraction Principles

Use short phrases only.

Avoid full sentences when possible.

Prefer compact keywords.

Extract from:

Introduction  
Literature Review  
Data  
Methods  
Results

Use only information stated in the paper or directly inferable from standard academic reporting.

If not clearly available, write none.

---

# Controlled Vocabulary Guidance

## Level of Analysis
Use one of:
Individual
Household
Regional
Country
none

## Gender Focus
Use one of:
Women
Men
Mixed
none

## Outcome Type
Examples:
Migration aspiration
Migration intention
Migration behavior
Fertility
Mortality
Labor market outcome
Education outcome
none

## Method Type
Examples:
Regression
Event history analysis
Multilevel model
Qualitative analysis
Mixed methods
none

## Model Specification
Examples:
Logit
Probit
OLS
Hazard model
Fixed effects
Random effects
Multinomial logit
Linear probability model
none

## Identification Strategy
Examples:
IV
Natural experiment
Matching
Panel fixed effects
Sister fixed effects
none

## Priority
Use only:
High
Medium
Low

## Read Status
Always output:
Not read

---

# Final Check Before Output

Before outputting, verify all of the following:

1. There is exactly one code block.
2. There are exactly two lines inside it.
3. Line 1 exactly matches the required header row.
4. Line 2 has exactly 25 tab-separated cells.
5. No cell is empty.
6. Any missing information is written as none.
7. Read Status is Not read.

---

# Output Template (Fill Only)

Always output using the following template.

Do NOT change column order.

Do NOT change column names.

Replace the bracket values only.

If information is missing, replace with:

none

Return the result inside one code block.

Template:

Paper	Year	Country/Region	Data Source	Data Type	Sample / Unit	Level of Analysis	Gender Focus	Theory	Research Question	Outcome Type	DV	Main IV	Controls	Mechanism	Method Type	Model Specification	Identification Strategy	Main Findings	Contribution	Key Theory References	Closely Related Studies	Research Gap	Priority	Read Status
[Paper]	[Year]	[Country/Region]	[Data Source]	[Data Type]	[Sample / Unit]	[Level of Analysis]	[Gender Focus]	[Theory]	[Research Question]	[Outcome Type]	[DV]	[Main IV]	[Controls]	[Mechanism]	[Method Type]	[Model Specification]	[Identification Strategy]	[Main Findings]	[Contribution]	[Key Theory References]	[Closely Related Studies]	[Research Gap]	[Priority]	Not read
