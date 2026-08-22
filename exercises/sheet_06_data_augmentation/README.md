# Exercise Sheet 6: Data Augmentation & Domain Shift Robustness

## Overview
Evaluates the robustness of the baseline classifier against distribution shifts and environmental degradation using synthetic data augmentations.

## Tested Perturbations
* **Lighting Shifts:** Color jitter (brightness and contrast variation).
* **Sensor Noise:** Gaussian blurring.
* **Occlusions:** Random cutout/erasing.

## Key Findings
* Analyzes model degradation under dirty sensor and changing weather conditions.
* Benchmarks classification accuracy across all perturbation profiles.