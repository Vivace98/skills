---
name: i-text-learning
description: Analyze Italian text and extract verbs, nouns, adjectives, and grammar structures with clear explanations in English for language learning.
---

# Italian Text Learning Scanner

This skill analyzes Italian text, dialogue, transcripts, or subtitles and extracts the most important linguistic elements for learning.

The input should always be treated as **natural language text**, not as isolated subtitle fragments.

The goal is to reveal how Italian works by identifying:

• verbs and their conjugation  
• common nouns and their gender  
• adjectives and agreement patterns  
• grammar structures appearing in the text  

All explanations must be written **in clear English**.

The analysis should **avoid sentence-by-sentence commentary** and instead organize results by linguistic category.

---

# Input

The user may provide:

- Italian text
- dialogue
- subtitles
- transcript
- paragraph

Example input:

Gli ho dato il libro ieri perché lo voleva leggere.

---

# Analysis Procedure

1. Read the entire text first.
2. Identify verbs, nouns, adjectives, and grammar structures.
3. Organize the results into four sections.
4. Avoid sentence-by-sentence explanations.
5. Avoid repeating the same grammar point multiple times.

The goal is **clear linguistic recognition and explanation**, not translation.

---

# Section 1 — Verbs

List verbs appearing in the text.

For each verb include:

- verb form appearing in the text  
- infinitive  
- tense  
- person/number  
- short explanation in English

Example format:

ho dato → dare | passato prossimo | 1st singular  

Explanation:  
This is the **passato prossimo** of *dare*. It describes a completed action in the past and is formed with *avere + past participle*.

voleva → volere | imperfetto | 3rd singular  

Explanation:  
The **imperfetto** expresses an ongoing or background action in the past. Here it describes what someone wanted to do.

Rules:

- focus on conjugation recognition
- provide a short explanation in English
- do not repeat the same verb unless the tense changes

---

# Section 2 — Common Nouns

Extract common nouns appearing in the text.

For each noun include:

- article if present
- gender
- plural form
- short explanation in English

Example:

il libro → masculine | plural: libri  

Explanation:  
*Libro* means “book”. It is a masculine noun. Many masculine nouns ending in **-o** form their plural with **-i**.

la macchina → feminine | plural: macchine  

Explanation:  
*Macchina* means “car” or “machine”. Feminine nouns ending in **-a** usually change to **-e** in the plural.

Rules:

- prioritize frequent or useful nouns
- avoid listing insignificant nouns

---

# Section 3 — Adjectives

List adjectives appearing in the text.

For each adjective include:

- base form
- agreement pattern
- explanation in English

Example:

rosso  

Agreement:  
rosso / rossa / rossi / rosse  

Explanation:  
Italian adjectives change form to match the **gender and number** of the noun they describe.

verde  

Agreement:  
verde / verdi  

Explanation:  
Some adjectives have the same form in masculine and feminine but change in the plural.

Rules:

- do not repeat the same adjective multiple times
- highlight agreement patterns

---

# Section 4 — Grammar Points

Identify grammar structures appearing in the text.

Rules:

- list each grammar point only once
- provide a short explanation in English
- prioritize structures useful for learners

Example output:

Grammar points in this text:

Passato prossimo  

Explanation:  
Used to describe completed past actions. It is formed with *avere or essere + past participle*.

Indirect object pronoun (gli)

Explanation:  
*Gli* means “to him” or “to her”. It replaces an indirect object and appears before the verb.

Imperfetto

Explanation:  
Used for background descriptions, repeated actions, or ongoing situations in the past.

---

# Style Rules

Follow these principles:

- Do not analyze sentence-by-sentence
- Do not repeat the same grammar pattern
- All explanations must be written in English
- Keep explanations concise and clear
- Prioritize high-frequency vocabulary
- Focus on understanding language structure

---

# Output Structure

Always organize the output in this order:

1. Verbs  
2. Common Nouns  
3. Adjectives  
4. Grammar Points
