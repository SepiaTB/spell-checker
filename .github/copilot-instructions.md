# 🧠 Copilot Instructions for Spell Checker Project

## 🎯 Project Goal
This project is a learning-focused implementation of a **spell checker** using classic algorithms and data structures, without artificial intelligence or language models.

The goal is to understand how real-world systems like IDE spell-checkers work internally through hands-on experience.

---

## 📚 Development Principles

- ✅ Prioritize **learning and understanding** over fast implementation.
- ✅ Prefer **simple, explicit** code and standard data structures (e.g. dictionaries, lists, trees).
- ✅ Document **why** an approach or algorithm is chosen (in Markdown files if needed).
- ✅ Keep third-party libraries to a minimum, and justify their use if included.
- ✅ Remember to follow the SOLID principles.
- ❌ Do not use AI models, ML libraries, or NLP toolkits (like spaCy, NLTK, Transformers, etc).

---

## 🧱 Architecture Guidelines

The system should include:

1. **Trie** data structure for fast word lookup.
2. **Morphological normalization** (e.g. remove `-ing`, `-ed`, `-s`) to reduce word variants.
3. **Levenshtein distance algorithm** to suggest corrections for misspelled words.
4. **Simple CLI** to test the system interactively.

---

## 🛠️ Coding Guidelines

- The code should be written in python.
- Include **inline comments** for all core logic.
- If a function uses a known algorithm (e.g., Levenshtein), add a docstring explaining how it works.
- When designing a module (e.g., `morphology.py`, `trie.py`), add a short `README.md` or section in the main project doc explaining:
  - What the module does
  - Why it was implemented that way
  - How it fits into the full system

---

## 🧪 Testing and Debugging

- Provide basic **unit tests** for each core module.
- Keep tests simple and descriptive.
- Avoid complex testing frameworks unless justified.

---

## ✍️ Markdown Documentation

For each key component or decision, include:
- The purpose of the component
- What data structure or algorithm it uses
- Why that approach was selected
- Limitations or trade-offs

Use a dedicated file like `docs/technical-notes.md` to store this if needed.

---

## 📦 Project Structure (expected)

Keep `docs/architecture.md` updated to reflect the project structure.

---

## 🧠 Final Reminder

Copilot should act as a **collaborative tutor**, not just a code generator.

---
