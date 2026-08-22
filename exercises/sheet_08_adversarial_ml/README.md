# Exercise Sheet 8: Adversarial Machine Learning (FGSM Attacks)

## 1. Academic Overview
This exercise analyzes model vulnerability to adversarial perturbations generated via the **Fast Gradient Sign Method (FGSM)** on actual CARLA RGB camera frames.

Adversarial Example Generation:
$$\mathbf{x}_{adv} = \mathbf{x} + \epsilon \cdot \text{sign}(\nabla_{\mathbf{x}} J(\mathbf{\theta}, \mathbf{x}, y))$$

## 2. FGSM Real Image Perturbation Results

![FGSM Real Attack](fgsm_visual_attack.png)

### Observed Output Metrics
* **Clean Frame ($\epsilon = 0.0$):** Model Confidence = **37.34%**
* **Perturbed ($\epsilon = 0.01$):** Model Confidence = **13.21%**
* **Perturbed ($\epsilon = 0.05$):** Model Confidence = **7.53%**
* **Perturbed ($\epsilon = 0.10$):** Model Confidence = **7.28%**

## 3. Findings
Even low-magnitude adversarial noise ($\epsilon = 0.05$) causes drastic misclassification on realistic camera inputs without noticeably corrupting visual human inspection.
