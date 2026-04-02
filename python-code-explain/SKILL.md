---
name: python-code-explain
description: Explain Python code used in statistics, demography, social science research, and machine learning workflows in a clear, structured, beginner-friendly way.
---

# Python Research Code Explain Skill

This skill explains Python code used in research workflows.

It is designed for users working in:

- statistics
- demography
- social science research
- survey data analysis
- machine learning for social data
- academic data analysis

The explanation prioritizes **conceptual understanding over programming complexity**.

It assumes the user may not be a professional programmer.

---

# When to Use This Skill

Use this skill when the user asks to:

- explain Python data analysis code
- interpret pandas / numpy workflows
- understand sklearn or statsmodels models
- understand how a script fits in a research pipeline
- connect code to statistical meaning
- understand variable construction and recoding
- interpret model output

Typical contexts include:

- survey data analysis
- demographic datasets
- statistical modeling
- regression analysis
- machine learning prediction
- feature construction
- data cleaning

---

# Output Structure

Always organize the explanation using the following structure.

---

## 1. Overall Purpose

Explain in simple terms:

- what this code is doing overall
- which stage of the research workflow it belongs to

Examples:

- data cleaning
- variable construction
- descriptive statistics
- regression modeling
- machine learning training
- prediction
- visualization
- exporting results

Also explain:

**what research question or analysis step this code contributes to.**

---

## 2. Packages and Tools

List the packages used and explain their role in this specific code.

Examples:

- pandas → data manipulation
- numpy → numerical computation
- statsmodels → statistical modeling
- sklearn → machine learning models
- matplotlib / seaborn → visualization
- scipy → statistical tools

When useful, group them:

Statistical / modeling packages  
Data manipulation packages  
Visualization packages  

---

## 3. Code Logic by Block

Break the code into logical blocks.

For each block explain:

Input  
What the code does  
Why it is needed  
Output / object created  
How the result is used later

Focus on **analysis logic**, not just syntax.

---

## 4. Key Lines Explained

Explain important lines in simple terms.

For each line:

Code  
What the syntax means  
What object is created or modified  
Why this line is important for the analysis

Do not assume the reader knows Python.

---

## 5. Analytical Meaning

Explain the **statistical or analytical meaning** behind the code.

### Method meaning

Why this method or model is used.

Examples:

- logistic regression
- random forest
- train-test split
- cross validation
- feature scaling

### Variable meaning

Explain what variables represent substantively.

Example:

education_high → indicator for tertiary education  
income_diff → subjective income difficulty

### Interpretation meaning

Explain how outputs should be interpreted.

Examples:

- regression coefficients
- predicted probabilities
- feature importance
- model accuracy

---

## 6. Common Confusions

Highlight things that often confuse beginners.

Examples:

- difference between DataFrame and Series
- inplace operations
- difference between fit and predict
- how pandas filtering works
- interpreting model output

---

## 7. Research Notes

Point out possible issues:

- missing values
- sample selection
- incorrect variable coding
- model assumptions
- reproducibility problems

---

## 8. Clean Summary

End with a simple summary:

What the code does  
What statistical idea it implements  
What the researcher should remember
