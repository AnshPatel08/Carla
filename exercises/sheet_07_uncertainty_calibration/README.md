# Exercise Sheet 7: Uncertainty Quantification & Cost-Optimal Decisions

## Overview
Evaluates model confidence calibration and risk-sensitive decision making using Expected Calibration Error (ECE) and cost matrices.

## Key Features
* **ECE Calculation:** Quantifies overconfidence using empirical accuracy vs. predicted probability binning.
* **Temperature Scaling:** Fits optimal temperature $T^*$ to rescale output logits and minimize calibration loss.
* **Cost Matrix Optimization:** Implements custom thresholding $\tau^* = \frac{C_{FP}}{C_{FN} + C_{FP}}$ prioritizing false negative reduction (pedestrian safety).