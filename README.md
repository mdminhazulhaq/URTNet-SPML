# URTNet-SPML
URTNet: Residual Encoder and Transformer Encoder Integrated 1D U-Net Model For Stress Monitoring On Resource-Constrained Platforms


## Overview

URTNet is a lightweight deep learning architecture for stress detection using Photoplethysmography (PPG) signals. It integrates a 1D U-Net with Residual Encoder (RE) and Transformer Encoder (TE) modules to learn complementary feature representations for classifying PPG signals into Normal and Stress categories.

## Datasets

- **CASTA**, and **WESAD** datasets.


## Data Preprocessing

- **Sampling Frequency:** 64 Hz.
- **Segmentation:** 10-second windows (640 samples per segment).
- **Normalization:** Z-score normalization.
- **Data Splitting:** Subject-wise data splitting for independent subject evaluation.

## Proposed Model

- **Architecture:** Hybrid 1D U-Net integrated with Residual Encoder (RE) and Transformer Encoder (TE).
- **Objective:** Developing deep-learning based Stress Monitoring algorithms for efficient and affordable healthcare solution.

### Proposed URTNet Architecture

![Proposed URTNet Architecture](URTNet_diagram.jpg)

*Figure 1. Proposed URTNet architecture integrating 1D U-Net, Residual Encoder, and Transformer Encoder.*

## Experimental Setup

- **Validation Strategy:** Leave-One-Subject-Out (LOSO) cross-validation.
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-score, ROC-AUC, and Cohen's Kappa.

## Experimental Results

URTNet model evaluated on  CASTA and WESAD datasets.
### CASTA Dataset

![Normalized Confusion Matrix for CASTA Dataset](Results_CASTA.jpg)

*Figure 2. Normalized confusion matrix for the CASTA dataset.*

### WESAD Dataset

![Normalized Confusion Matrix for WESAD Dataset](Results_WESAD.jpg)

*Figure 3. Normalized confusion matrix for the WESAD dataset.*

## Embedded Deployment

The PPG-based stress detection research includes deployment on resource-constrained platforms:

- Raspberry Pi 3B+
- Arduino Nano BLE

## Code Availability

This repository provides an overview of the proposed URTNet architecture, datasets, preprocessing methodology, experimental setup, and research results.

The complete source code and full model implementation will be available following publication of the associated research paper.



## Copyright

Copyright © 2026 Md. Minhazul Haq. All rights reserved.

The materials in this repository are provided for research and academic reference. Reproduction, redistribution, or modification requires prior written permission from the copyright holder, except where permitted by applicable law.
