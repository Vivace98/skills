---
name: r-code-explain
description: Explain R code for statistics and research workflows, with structured logic, line-by-line guidance when needed, and statistical interpretation.
---

# R Code Explain Skill

This skill explains R code in a clear, structured, research-oriented way.

It is designed for users working in:
- statistics
- social science
- demography
- data analysis
- academic research

Use this skill when the user asks to:
- explain an R script
- interpret R code line by line
- understand a model specification in R
- understand packages and functions used in an R workflow
- connect code to statistical meaning

---

# Output Structure

Always organize the explanation using the following structure.

## 1. Overall Purpose
What is this code trying to do overall?

Examples:
- data cleaning
- variable construction
- descriptive analysis
- regression modeling
- survey-weighted estimation
- visualization
- exporting results

## 2. Packages and Tools
List the packages used and briefly explain what each one is doing.

Examples:
- dplyr → data manipulation
- ggplot2 → visualization
- survey → complex survey design and weighted estimation
- haven / readr → data import
- marginaleffects → marginal effects
- broom → model output formatting

## 3. Code Logic by Block
Break the code into meaningful blocks.
For each block:
- describe what it does
- explain why it appears here
- explain what the output of that block becomes

## 4. Line-by-Line Explanation (when useful)
If the code is short or the user asks for detailed explanation, explain line by line.

For each important line:
- explain the syntax
- explain the function
- explain the object created or modified

## 5. Statistical Meaning
Explain the statistical meaning behind the code, not just the programming meaning.

Examples:
- why a logistic regression is used
- what survey weights are doing
- what a factor recode changes substantively
- what an interaction term means
- what average marginal effects represent

## 6. Common Mistakes or Confusions
Point out possible misunderstandings.

Examples:
- confusing filtering with selecting
- misunderstanding mutate vs summarise
- forgetting reference categories in factors
- confusing coefficients with marginal effects
- misunderstanding weighted vs unweighted results

## 7. Clean Summary
End with a short summary:
- what the code does
- what the key statistical idea is
- what the user should remember

---

# Style Rules

- Default language: Chinese
- Start with the big picture, then move to details
- Use clear section titles
- Be precise but not overly dense
- If the user is learning, prioritize understanding over brevity
- If the code involves statistics, always explain the statistical logic
- If the code is part of a research workflow, explain where it sits in the workflow

---

# Special Notes

When the code includes:
- `glm`, explain link function, response type, and interpretation logic
- `lm`, explain linear model assumptions and coefficient meaning
- `svydesign` or `svyglm`, explain survey design and weighted inference
- `mutate`, `case_when`, `factor`, explain variable construction carefully
- `ggplot`, explain what each layer is doing
- `forcats`, explain reference categories if relevant

If the user asks for line-by-line explanation, be thorough.
If the code is long, first split it into logical blocks, then explain each block clearly.
