# 🌿 ArvyaX ML Assignment
**Kritarth Joshi**

## Objective
Build a system that:
- Understands emotional state
- Predicts intensity
- Recommends actions (what + when)
- Handles uncertainty

---

## Approach

### 1. Data Processing
- Text processed using TF-IDF
- Metadata features included (sleep, stress, energy, etc.)
- Missing values handled:
  - Numerical → median
  - Categorical → most frequent

---

### 2. Modeling

#### Emotional State
- Model: Logistic Regression
- Reason: works well for text classification and interpretable

#### Intensity
- Model: Random Forest Regressor
- Reason: handles non-linear relationships and ordinal nature

---

### 3. Decision Engine

Rule-based system using:
- stress level
- energy level
- sleep

Examples:
- High stress + low energy → rest
- High energy + low stress → deep work
- High stress → breathing

---

### 4. Uncertainty Handling
- Confidence = max probability
- If confidence < 0.6 → uncertain_flag = 1

---

### 5. Ablation Study

| Model | Performance |
|------|------------|
| Text only | Lower |
| Text + metadata | Better |

Conclusion:
Metadata significantly improves performance.

---

## How to Run

1. Place train.csv and test.csv in same folder
2. Run notebook
3. predictions.csv will be generated

---

## Output Format

- predicted_state  
- predicted_intensity  
- confidence  
- uncertain_flag  
- what_to_do  
- when_to_do  

---

## Key Strengths

- Handles noisy text
- Uses contextual signals
- Provides actionable recommendations
- Includes uncertainty awareness
