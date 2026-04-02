---

name: italian-text-scanner
description: Scan Italian text, dialogue, or subtitles and extract verbs with conjugations, common nouns with gender, adjectives, and unique grammar patterns for language learning.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Italian Text Scanner

This skill analyzes Italian text, dialogue, transcripts, or subtitles and extracts the most important linguistic elements for learning.

The input should always be treated as **natural language text**, not as isolated subtitle fragments.

The goal is to quickly reveal the structure of the language by identifying:

• verbs and their conjugation
• common nouns and their gender
• adjectives
• grammar patterns appearing in the text

The analysis should **avoid sentence-by-sentence commentary** and instead organize results by linguistic category.

---

# Input

User may provide:

• Italian text
• dialogue
• subtitles
• transcripts
• paragraphs

Example:

Gli ho dato il libro ieri perché lo voleva leggere.

---

# Analysis Procedure

Read the entire text first.

Then extract linguistic elements and organize them into four sections.

Do not analyze sentence-by-sentence.

Avoid repeating the same grammar point multiple times.

Prioritize **recognition and learning efficiency** over long explanations.

---

# Section 1 — Verbs

List verbs appearing in the text.

For each verb include:

• verb form appearing in the text
• infinitive
• tense
• person/number

Example format:

ho dato → dare | passato prossimo | 1st singular
voleva → volere | imperfetto | 3rd singular
arrivi → arrivare | congiuntivo presente | 3rd singular

Focus on **recognizing conjugation patterns**.

Do not repeat the same verb multiple times unless the tense changes.

---

# Section 2 — Common Nouns

Extract common nouns appearing in the text.

For each noun include:

• article if present
• gender
• plural form if useful

Example:

il libro → masculine | plural: libri
la macchina → feminine | plural: macchine
la bandiera → feminine | plural: bandiere

Prioritize **frequent or useful nouns**, not every noun in the text.

---

# Section 3 — Adjectives

List adjectives appearing in the text.

For each adjective include:

• base form
• agreement examples if visible

Example:

rosso → rossa / rossi / rosse
nero → nera / neri / nere
verde → invariant in singular, plural: verdi

Do not repeat the same adjective multiple times.

---

# Section 4 — Grammar Points

Identify grammar structures appearing in the text.

Rules:

• list each grammar point only once
• explanations should be short
• prioritize structures useful for learners

Examples:

passato prossimo
imperfetto
reflexive verbs
direct object pronouns
indirect object pronouns
subjunctive clauses
preposition + article combinations

Example output:

Grammar points in this text:

• passato prossimo
• indirect object pronouns (gli)
• imperfetto for background description

---

# Style Rules

Follow these principles:

• Do not analyze sentence-by-sentence
• Do not repeat the same grammar pattern
• Avoid unnecessary linguistic theory
• Keep explanations concise
• Prioritize high-frequency vocabulary
• Focus on recognition rather than translation

The output must always follow this structure:

1. Verbs
2. Common Nouns
3. Adjectives
4. Grammar Points
