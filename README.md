# 🧠 Spell Checker without AI

This is a learning-focused project that aims to build a **spell checker from scratch**, using only **classic algorithms and data structures**, without relying on any artificial intelligence systems.

The project is inspired by how traditional spell checkers work in text editors and IDEs (like Word or VSCode), as explained in [this video](https://www.instagram.com/reel/DLGC8FjzFiw/?igsh=MXY0M25idm9tb203MA==).

---

## 🎯 Goal

Develop a system capable of:

- Verifying if a word is correctly spelled.
- Applying morphological rules to recognize variants such as plurals or verb tenses.
- Suggesting possible corrections for misspelled words.
- Doing all of this efficiently using optimized structures.

---

## ⚙️ Technologies and Principles

This project **does not use language models or machine learning**. It relies on:

- **Trie (prefix tree):** to store a dictionary and quickly check word existence.
- **Morphological rules:** to normalize words like `running` → `run`.
- **Levenshtein distance:** to suggest similar words when a typo is detected.
- **Lexical analysis:** to prioritize more common words as suggestions.

---

## 🧩 System Components

### 1. Trie (the core structure)
A tree-based structure that allows verifying if a word exists without scanning the entire dictionary.

```plaintext
To verify "code":
C → O → D → E (4 hops)
vs.
171,000 comparisons in a list
```

---

### 2. Morphological Rules
A simple rule engine that reduces a word to its base form before looking it up.

Examples:
- `"running"` → `"run"`
- `"played"` → `"play"`
- `"dogs"` → `"dog"`

---

### 3. Suggestion Engine
If a word is not found:

- Candidate words are retrieved with similar length or prefix.
- Their **Levenshtein distance** from the input word is calculated.
- Suggestions are sorted by similarity and frequency.

---

### 4. CLI Interface (future)
An interactive command-line interface to test the checker:

```bash
> python corrector.py
Enter a word: runing
Did you mean?: running, ruining, ruling
```

---

## 🧪 Project Status

Development is organized into **epics and user stories**, tracked via GitHub Projects. Each module is valuable on its own.

Planned epics:

- [x] Trie structure and word verification
- [ ] Morphological normalization
- [ ] Similar prefix/length suggestion engine
- [ ] Levenshtein distance calculator
- [ ] CLI interface

---

## 🤓 Learning Focus

This project is designed to deepen understanding of:

- Efficient data structures
- Classic algorithms applied to real-world problems
- Correction systems without artificial intelligence

Perfect as an educational or technical demonstration.

---

## 📂 Repository Structure

```
/corrector/
  ├── trie.py              # Trie implementation
  ├── morphology.py        # Morphological rules
  ├── levenshtein.py       # Distance calculation
  ├── corrector.py         # Main entry point
  └── tests/               # Unit tests
```

---

## 🛠️ Contributing

This is a personal project, but if you'd like to contribute:

1. Open an issue with ideas or feedback.
2. Submit a pull request with fixes or features.
