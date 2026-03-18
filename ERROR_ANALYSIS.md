# ❌ Error Analysis

## 1. Short Text
Example: "ok", "fine"
- Problem: insufficient signal
- Result: incorrect prediction

---

## 2. Ambiguous Text
Example: "idk how I feel"
- Problem: unclear emotion
- Result: model confusion

---

## 3. Contradictory Signals
Example:
- Text: calm
- Stress: high

- Problem: conflicting inputs
- Result: inconsistent prediction

---

## 4. Noisy Labels
Some training labels may not match text exactly.

---

## 5. Vague Reflections
Example: "it was okay"
- No clear emotional signal

---

## Improvements

- Use contextual embeddings (BERT)
- Add more data
- Improve label quality
- Use sequence models