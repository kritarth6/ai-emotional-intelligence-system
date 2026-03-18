# 📱 Edge Deployment Plan

## Goal
Deploy system on mobile / low-resource environment

---

## Model Choice
- TF-IDF (lightweight)
- Logistic Regression (small size)
- Random Forest (moderate size)

---

## Optimization

- Reduce TF-IDF features (3000 → 1000)
- Compress model
- Use ONNX / quantization

---

## Latency
- Fast inference (<100ms)
- Suitable for real-time feedback

---

## Tradeoffs

| Factor | Tradeoff |
|------|---------|
| Accuracy | Slightly reduced |
| Speed | Improved |
| Size | Reduced |

---

## Handling Edge Cases

- Short text → fallback rule
- Missing values → default values
- Uncertain predictions → flag

---

## Future Improvements

- Use lightweight transformers
- Personalization
- On-device fine-tuning