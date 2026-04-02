---
name: paper-research-core
description: 学术论文深度解析工具。用于 demography、statistics、social science 论文阅读。每当用户上传论文 PDF、粘贴论文文本、或请求分析 research question / literature review / data / methods / research design 时优先使用此 skill。
---

# Paper Research Core — 学术论文深度解析工具

This skill analyzes academic papers following a researcher's reading logic.

It is designed for demography, migration, social science, and statistical research workflows.

The goal is **not only to summarize**, but to reconstruct the **research logic of the paper**.

---

# When to Use

Use this skill when the user:

- uploads a research paper PDF
- asks to analyze a paper
- asks for literature review notes
- wants to understand research design
- wants to extract data, method, or modeling structure

Typical requests:

- "summarize this paper"
- "analyze this article"
- "make literature review notes"
- "explain the research design"

---

# Evidence Discipline (Important)

All summaries must be grounded in the **original text of the paper**.

Distinguish clearly between:

1. statements explicitly made by the authors
2. reasonable paraphrases from the text
3. critical interpretation

If the paper does not clearly state something (e.g., assumption, mechanism), write:

"论文未明确说明"

Do not fabricate information.

Whenever possible, mention the section where the information comes from:

- Introduction
- Literature Review
- Data
- Methods
- Results
- Discussion

---

# Output Language

Output must be written in **Chinese**, unless the user explicitly requests another language.

---

# Output Structure

Always produce the following structured research notes.

---

# 1 研究问题 (Research Question)

- 这篇论文试图回答什么问题？
- 这个问题属于哪个更大的研究议题？
- 作者为什么认为这个问题重要？

---

# 2 文献综述与研究缺口 (Literature Review & Research Gap)

- 文献综述的逻辑结构是什么？
- 作者引用了哪些关键文献？
- 学术界的主要争论是什么？
- 作者认为现有研究缺少什么？
- 研究问题是如何从文献综述中提出的？

如果论文没有清晰提出 research gap，需要说明。

---

# 3 数据与研究对象 (Data & Research Object)

提取：

- 数据来源
- 国家 / 地区
- 时间范围
- 样本规模
- 研究单位 (individual / household / region 等)

同时说明：

研究对象是什么？

例如：

- fertility
- migration
- mortality
- labor outcomes

---

# 4 变量与研究设计 (Variables & Research Design)

识别：

- 因变量 (dependent variable)
- 核心解释变量 (key explanatory variables)
- 控制变量 (controls)

如果论文没有明确说明变量构建方式，需要指出。

---

# 5 方法与建模 (Methods & Modeling)

提取：

- 使用的方法  
  (例如 regression / event history analysis / DID / qualitative)

- 模型结构

例如：

- logistic regression
- hazard model
- fixed effects model

解释：

为什么这种方法适合研究问题？

如果存在 identification strategy，需要说明。

---

# 6 假设与识别逻辑 (Assumptions & Identification)

分析：

- 研究依赖哪些关键假设？
- 识别策略是什么？
- 是否存在潜在偏误？

例如：

- selection bias
- omitted variable bias
- reverse causality

如果论文没有讨论这些，需要指出。

---

# 7 核心发现 (Main Findings)

用 bullet points 总结：

- 最重要的实证结果
- 是否存在异质性
- 是否提出机制解释

尽量基于 Results / Discussion。

---

# 8 结论是否被支持 (Are Conclusions Supported?)

批判性判断：

- 论文结论是否真正被结果支持？
- 是否存在过度解释？
- 是否存在证据不足的地方？

---

# 9 研究贡献 (Research Contribution)

从三个角度说明：

- 理论贡献
- 实证贡献
- 方法贡献

---

# 10 局限与未来研究 (Limitations & Extensions)

识别：

- 数据局限
- 方法局限
- 外推性问题

并说明未来研究可以如何扩展。

---

# 11 与用户研究的关联 (Relevance to User's Research)

解释该论文如何与以下主题相关：

- migration
- demography
- gender
- social inequality
- fertility

同时说明：

这篇论文在 literature review 中可以如何引用。

---

# Style Rules

- Academic tone
- Structured bullet points
- Concise but precise
- Avoid unnecessary verbosity

---

# Goal

Transform academic papers into **structured research notes** that can be directly reused for:

- literature review
- thesis preparation
- research design learning

# Quotation Rule

When possible, briefly quote or paraphrase key sentences from the paper and indicate the section (e.g., Introduction, Results).
