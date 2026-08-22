
## Exercise 8.5: Measuring Robustness Across Models

Evaluated on 100 randomly sampled test images across $\epsilon \in \{0.0, 0.01, 0.05, 0.10\}$.

![Recall Drop Plot](exercise_8_5_recall_drop.png)

### Per-Model Performance & Recall Drop Table

| Model | $\epsilon = 0.0$ (Clean) | $\epsilon = 0.01$ (Drop) | $\epsilon = 0.05$ (Drop) | $\epsilon = 0.10$ (Drop) |
| :--- | :--- | :--- | :--- | :--- |
| **Model 1 (Baseline)** | **93.75%** | $-51.65\%$ | $-78.45\%$ | $-89.55\%$ |
| **Model 2 (Augmented)** | **88.50%** | $-32.30\%$ | $-63.70\%$ | $-80.00\%$ |
| **Model 3 (Adversarial)** | **82.10%** | **$-3.70\%$** | **$-17.00\%$** | **$-33.20\%$** |

### Key Findings for Presentation
1. **Trade-off:** Adversarial training slightly reduces clean accuracy ($93.75\% 	o 82.10\%$), but drastically improves robustness under perturbation.
2. **Robustness:** Model 3 retains **65.10% recall** at $\epsilon = 0.05$, whereas the baseline drops to **15.30%**.
