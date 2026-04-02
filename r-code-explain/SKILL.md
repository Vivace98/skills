---
name: r-code-explain
description: Explain R code for statistics, demography, and research workflows with structured logic, statistical meaning, and workflow context.
---

# R Code Explain Skill

This skill explains R code in a clear, structured, research-oriented way.

It is designed for users working in:
- statistics
- social science
- demography
- survey data analysis
- academic research

Use this skill when the user asks to:
- explain an R script
- interpret R code line by line
- understand a model specification in R
- understand packages and functions used in an R workflow
- connect code to statistical meaning
- understand where a code block fits in the research pipeline

---

# Output Structure

Always organize the explanation using the following structure.

## 1. Overall Purpose
Explain:
- what this code is doing overall
- which stage of the research workflow it belongs to
- what result, dataset, model, table, or figure it is trying to produce

Examples:
- data cleaning
- variable construction
- descriptive analysis
- regression modeling
- survey-weighted estimation
- visualization
- exporting results
- robustness checks

## 2. Packages and Tools
List the packages used and explain what each one is doing in this specific code.

Examples:
- dplyr → data manipulation
- ggplot2 → visualization
- survey → complex survey design and weighted estimation
- haven / readr → data import
- marginaleffects → marginal effects
- broom → model output formatting
- forcats → factor handling and reference levels

When relevant, distinguish:
- statistical core packages
- data wrangling packages
- output / plotting packages

## 3. Code Logic by Block
Break the code into meaningful blocks.

For each block, explain:
- Input: what object(s) it starts from
- What it does
- Why it appears here
- Output / object created
- How that output is used later in the workflow

## 4. Line-by-Line Explanation
Use detailed line-by-line explanation when:
- the user explicitly asks for it
- the code is short
- a block contains important recoding, modeling, or interpretation logic

For each important line:
- explain the syntax
- explain the function
- explain the object created, modified, or overwritten
- explain any important defaults or hidden assumptions

## 5. Statistical Meaning
Explain the statistical meaning behind the code, not just the programming meaning.

Cover these levels when relevant:
- Method meaning: why this method/model is used
- Variable meaning: what the coding or recoding means substantively
- Interpretation meaning: how the resulting coefficients, predictions, or outputs should be interpreted

Examples:
- why a logistic regression is used
- what survey weights are doing
- what a factor recode changes substantively
- what an interaction term means
- what average marginal effects represent
- what a reference category implies
- what this model output contributes to the research question

## 6. Common Mistakes or Confusions
Point out likely misunderstandings.

Examples:
- confusing filter with select
- misunderstanding mutate vs summarise
- forgetting reference categories in factors
- confusing coefficients with marginal effects
- misunderstanding weighted vs unweighted results
- treating recoded variables as equivalent to original raw variables
- interpreting associations as causal effects without justification

## 7. Research Risks or Notes
When useful, point out possible issues in the code or workflow.

Examples:
- reference category may not match the research narrative
- recoding may hide missing values
- model specification may omit needed controls
- survey design may be partially specified
- plot labels may not match variable meaning
- exported results may be hard to reproduce later

## 8. Clean Summary
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
- If the code is long, first split it into logical blocks, then explain block by block
- If the user asks for line-by-line explanation, be thorough and do not skip key lines

---

# Special Notes

When the code includes:
- `glm`, explain response type, link function, coefficient logic, and interpretation limits
- `lm`, explain model assumptions and coefficient meaning
- `svydesign` or `svyglm`, explain survey design, weights, PSU/strata if present, and weighted inference
- `mutate`, `case_when`, `if_else`, `factor`, explain variable construction carefully
- `relevel` or `forcats`, explain reference categories explicitly
- `ggplot`, explain what each layer is doing and what the figure is meant to show
- `marginaleffects`, explain the difference between coefficients and marginal effects
- model comparison code, explain what exactly is being compared and why
- exported tables/figures, explain how they relate to the research output
