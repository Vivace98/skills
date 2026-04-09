# Tarot Workspace Agent

This directory is used for daily tarot reflection.

The workflow is simple:

1. Draw three random cards from the Rider-Waite deck.
2. Show the cards.
3. Ask the user whether they want a simple interpretation.
4. If yes, interpret the cards using `simple-reading.md`.

---

# Files in this directory

rider-waite-cards.md  
→ Contains the meanings of all 78 Rider-Waite tarot cards.

simple-reading.md  
→ Instructions for generating short interpretations.

tarot-agent.md  
→ This file. Explains how the tarot workspace should operate.

---

# Card Drawing Rules

Draw 3 cards randomly.

Each card has a 30% chance of being reversed.

Examples:

The Hermit  
The Star  
Three of Cups (Reversed)

---

# Interpretation Rules

If the user asks for interpretation:

1. Look up the card in `rider-waite-cards.md`.
2. Use upright meaning if upright.
3. Use reversed meaning if reversed.
4. Convert the meaning into **one short reflective sentence**.

Tone guidelines:

- calm
- reflective
- non-predictive
- concise

Tarot is treated as a **daily reflection tool**, not a fortune-telling system.
