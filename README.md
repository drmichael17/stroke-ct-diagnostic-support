# AI-Powered CT Diagnostic Support for Stroke

Deep-learning-based diagnostic support for classification of brain CT images, developed with an emphasis on clinically relevant stroke classification, model comparison, validation, explainability, and deployable decision support.

## Overview

This repository contains the research code for an AI-assisted stroke diagnostic-support project using brain CT imaging.

The system investigates both direct multiclass classification and a hierarchical classification framework for distinguishing:

- Normal CT
- Hemorrhagic stroke
- Ischemic stroke
- Other intracranial abnormalities

The project was designed to explore how deep learning can support CT-based stroke assessment while maintaining a pathway toward practical clinical deployment.

## Models

The implementation includes transfer-learning experiments using:

- EfficientNetB0
- MobileNetV2

Two classification strategies are explored:

1. Direct four-class classification
2. Hierarchical classification:
   - Stage 1: Stroke-related vs. other abnormalities
   - Stage 2: Normal vs. hemorrhagic vs. ischemic CT

## Technical Features

The notebook includes:

- CT image preprocessing
- Reproducible train-validation splitting
- Data augmentation
- Class weighting for imbalanced datasets
- Transfer learning
- Fine-tuning
- Early stopping
- Learning-rate reduction
- Confusion-matrix analysis
- Precision, recall, F1-score, and accuracy evaluation
- Grad-CAM-based model interpretation
- Comparative model evaluation

## Validation

In the hierarchical experiments contained in the notebook, EfficientNetB0 achieved the strongest validation performance among the evaluated architectures.

The notebook also includes an independent external-test component to support evaluation beyond the development split.

## Explainability

Grad-CAM is incorporated to visualize image regions contributing to model predictions and to support interpretation of the deep-learning classifier.

## Clinical Translation

The broader project extends beyond model development to deployment as a Telegram-based diagnostic-support tool, demonstrating a pathway from model experimentation to accessible clinical decision support.

This system is intended for research and decision-support purposes and is not a replacement for radiological or clinical diagnosis.

## Repository Contents

`stroke_ct_diagnostic_support.ipynb`

Main research notebook containing dataset preparation, model training, validation, evaluation, explainability, and hierarchical classification experiments.

## Publication

This work is associated with the peer-reviewed study:

**Ogunmiloro B. Artificial intelligence (AI)-powered diagnostic support for stroke via Telegram bot: preliminary findings. BMC Neurology. 2026.**

## Author

**Babatunde Ogunmiloro, M.D.**  
Medical doctor and applied biomedical AI researcher

Research interests include medical image analysis, clinical artificial intelligence, deep learning, external validation, and deployable decision-support systems.
