---
name: italian-dialogue-learning
description: Analyze Italian subtitles or short texts by identifying verbs, conjugations, noun gender, adjectives, and grammar points, then classify them by CEFR level.
---

# Italian Subtitle Analyzer

Use this skill when the user provides:
- Italian subtitles
- short Italian dialogue
- short Italian text
- lines from films, series, YouTube videos, podcasts, or transcripts

The goal is to help a learner rebuild Italian grammar intuition after forgetting part of the grammar system.

## Priorities

Always focus on these in order:

1. verbs and conjugation
2. pronouns and clitics
3. noun gender and number
4. adjectives
5. grammar points
6. CEFR level classification
7. simplified learner explanation

## Output rules

Always analyze the text line by line.

For each line, produce the following sections.

### 1. Original line
Copy the original Italian line.

### 2. Segmentation
Break the line into meaningful parts.

Example:
`Ci | vado | domani`

### 3. Verb analysis
Identify every verb and report:

- surface form
- infinitive
- tense
- mood
- person and number
- short meaning in context

Example:
- `vado` → `andare`, present indicative, 1st person singular, “I go”

If the line has auxiliaries or compound tenses, explain the structure clearly.

Example:
- `ho dato` → passato prossimo of `dare`

### 4. Pronouns and small grammar words
Identify items such as:
- ci
- ne
- lo / la / li / le
- gli
- mi / ti / si / ci / vi

Explain:
- what type they are
- what they refer to if clear from context
- what function they have in the sentence

### 5. Nouns and adjectives
Identify common or important nouns and adjectives.

For each noun, report:
- article if present
- gender
- singular/plural form
- meaning

For each adjective, report:
- base form
- agreement if relevant
- meaning

### 6. Grammar points
Explain the grammar structures that appear in the line.

Examples:
- present indicative
- passato prossimo
- reflexive verb
- direct object pronoun
- indirect object pronoun
- partitive pronoun
- preposition + article
- adjective agreement

Keep the explanation simple and learner-friendly.

### 7. CEFR tag
Tag each important grammar point as roughly:
- A1
- A2
- B1
- B2+

Use practical teaching judgment, not strict exam taxonomy.

### 8. Learner note
At the end of each line, add:
- what is most important for the learner to notice
- what is easy to confuse
- one very short memory tip if useful

## Global summary

After analyzing all lines, provide four short summary blocks:

### A. Verbs to remember
List the most useful verbs and their infinitives.

### B. Pronoun/clitic patterns to review
List the pronouns or clitic structures that appear.

### C. Core vocabulary
List the most useful nouns and adjectives.

### D. Study priority for this text
Classify the text overall:
- mostly A-level
- A-level with some B1
- mostly B1
- B1 with B2 features

## Style rules

- Be concrete, not abstract.
- Prioritize clarity over linguistic theory.
- Do not overwhelm the learner with unnecessary terminology.
- If a structure is ambiguous, say so.
- If the text is subtitle-like and incomplete, explain based on the available context only.
- Prefer short examples over long explanations.
- For this learner, especially highlight:
  - verb conjugation
  - pronouns/clitics
  - noun gender
  - singular/plural patterns

## When simplifying

If the user seems confused, add a final section:

### Simplified version
Rewrite the line in simpler Italian where possible, while preserving the meaning.

## Learner profile

The learner previously studied Italian grammar to around B2 level, but has forgotten part of it after a long pause.

Current difficulties:
- recognizing verb conjugations quickly
- understanding pronouns and clitics
- remembering noun gender and plural patterns

Therefore:
- prioritize structural decoding over long explanations
- make morphology visible
- keep explanations simple and practical
- point out what should be reviewed, not everything that could be said
