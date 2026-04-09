---
name: tarot
description: Draw three random Rider-Waite tarot cards for daily reflection and optionally provide a simple interpretation.
---

# Daily Tarot Skill

This skill draws three random tarot cards for daily reflection.

The purpose is **not prediction**, but **symbolic reflection**.

The workflow is intentionally simple:

1. Draw three random cards from the Rider-Waite deck.
2. Show the cards.
3. Ask whether the user wants a simple interpretation.
4. If yes, read the file `simple-reading.md` in the tarot workspace.

No deep analysis is provided automatically.

---

# Workflow

When the user activates the tarot skill:

## Step 1 — Draw Cards

Randomly draw three cards from the Rider-Waite deck.

Each card has:

- name
- optional reversed orientation (30% probability)

Example output:

Today's tarot draw

1. The Hermit  
2. Three of Cups (Reversed)  
3. The Star  

Do not interpret yet.

---

## Step 2 — Ask for interpretation

Ask the user:

Would you like a simple interpretation? (yes / no)

---

## Step 3 — If user says yes

Read the file:

tarot/simple-reading.md

Then generate a **short interpretation** for each card using the meanings from:

tarot/rider-waite-cards.md

Rules:

- 1 sentence per card
- calm tone
- reflective, not predictive
- no dramatic language

Example format:

Simple interpretation

Card 1 — The Hermit  
today may invite quiet reflection and solitude.

Card 2 — Three of Cups (Reversed)  
social energy may feel slightly drained.

Card 3 — The Star  
hope and healing are quietly returning.

---

# Principles

Tarot here is used as a **mirror**, not a prophecy.

The interpretation should:

- remain neutral
- encourage reflection
- avoid deterministic statements
- avoid predicting future events
