# bday 🎂
A rule-based conversational program built to explore intent detection, response memory, and incremental intelligence in simple systems.

---

## Problem
Most beginner chatbots and conversational programs respond statically:
they react, but they do not *remember*, *adapt*, or *evolve*.

This project was built to study:
- how basic intent matching works
- how short-term memory affects responses
- how small upgrades can meaningfully improve interaction quality

The goal is not realism, but **understanding**.

---

## Approach
The system uses a lightweight, rule-based approach instead of heavy ML models.

Core ideas:
- detect intent using keywords
- prioritize responses using simple weighting
- remember the last interaction to influence future replies

This keeps the system transparent and easy to reason about.

---

## Logic Flow
1. Take user input
2. Normalize input (lowercase, trim, tokenize)
3. Match keywords to known intents
4. Rank intents based on keyword frequency
5. Generate response
6. Store last response in memory
7. Adjust next reply using memory context

This flow emphasizes *why* decisions are made, not just what happens.

---

## Limitations
- No deep language understanding
- Keyword-based matching can misinterpret intent
- Memory is short-term and volatile
- No learning persists across sessions

These limits are intentional to keep behavior explainable.

---

## Future Upgrades
- Weighted keyword scoring instead of binary matching
- Intent confidence thresholds
- Persistent memory (file-based or database)
- Emotion tagging for responses
- Transition to lightweight NLP libraries

---

## Evolution Story
- v0.1: Static responses
- v0.2: Keyword-based intent detection
- v0.3: Last-response memory added
- v0.4: Response prioritization

Each version reflects a specific learning milestone.
