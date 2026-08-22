# Exercise Sheet 8: Adversarial Machine Learning (FGSM)

## Overview
Investigates model vulnerability to gradient-based adversarial attacks using the **Fast Gradient Sign Method (FGSM)**.

## Key Evaluation
* **Attack Method:** $\mathbf{x}_{adv} = \mathbf{x} + \epsilon \cdot \text{sign}(\nabla_{\mathbf{x}} J(\mathbf{\theta}, \mathbf{x}, y))$.
* **Epsilon Sweep:** Performance breakdown under $\epsilon \in \{0.01, 0.05, 0.1\}$.
* **Metrics Tracked:** Qualitative visual comparisons (Clean vs. Adversarial) and Recall Drop percentage under attack.