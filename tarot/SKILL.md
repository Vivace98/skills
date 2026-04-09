---
name: tarot
description: Draw three random Rider-Waite tarot cards for daily reflection and optionally provide a simple interpretation.
---

# Daily Tarot Skill

This skill is a minimal daily tarot reflection tool.

It does only one thing:

- draw 3 random Rider-Waite tarot cards
- optionally give a simple interpretation

Tarot here is used as a symbolic mirror, not as prediction.

---

## Workspace

The tarot workspace contains these files:

- `tarot/cards-list.md`
- `tarot/rider-waite-cards.md`
- `tarot/simple-reading.md`
- `tarot/tarot-agent.md`

Use them when running this skill.

---

## Workflow

### Step 1 — Draw 3 cards

Use `tarot/cards-list.md` as the official deck list.

Rules:

- draw exactly 3 different cards
- no repeated cards
- each card has a 30% chance of being reversed
- show the cards first without interpretation

Use this output format:

Today's tarot draw

1. [Card Name]
2. [Card Name]
3. [Card Name]

If reversed, write:

[Card Name] (Reversed)

---

### Step 2 — Ask for simple interpretation

After showing the 3 cards, ask:

Would you like a simple interpretation? (yes / no)

---

### Step 3 — If the user says yes

Read:

- `tarot/simple-reading.md`
- `tarot/rider-waite-cards.md`

Then generate a short interpretation.

Rules:

- one short sentence per card
- calm and reflective tone
- no prediction
- no dramatic wording
- focus on today's energy or reflection

Use this format:

Simple interpretation

Card 1 — [Card Name]  
[One short reflective sentence]

Card 2 — [Card Name]  
[One short reflective sentence]

Card 3 — [Card Name]  
[One short reflective sentence]

---

## Principles

This skill should remain:

- simple
- steady
- reflective
- non-predictive

Do not add deep analysis unless explicitly requested outside this workflow.
