# Exercise Sheet 9: Out-of-Distribution (OOD) Detection

## Overview
Implements out-of-distribution detection to flag unmapped environments (fog, night, and unseen towns) before making unsafe driving decisions.

## Detectors Benchmark
1. **Maximum Softmax Probability (MSP):** Baseline output-confidence anomaly score.
2. **k-NN Feature Distance:** Distance measurement on deep feature representations extracted from the penultimate ResNet layer.
* **Metrics Tracked:** AUROC comparisons for detecting distribution shifts.