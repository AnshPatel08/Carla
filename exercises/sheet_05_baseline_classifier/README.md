# Exercise Sheet 5: Baseline Pedestrian Classifier

## Overview
This module implements a baseline binary pedestrian classification model using **ResNet18** fine-tuned on CARLA simulator front-camera RGB images.

## Key Features & Outputs
* **Model Architecture:** Pre-trained ResNet18 with modified final fully-connected output layer ($1$ logit output).
* **Evaluation Metrics:** ROC-AUC score, Precision, Recall, F1-Score, and Confusion Matrix.
* **Outputs Generated:**
  * Performance classification report.
  * Receiver Operating Characteristic (ROC) Curve plot.