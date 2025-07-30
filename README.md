# Neural Networks for 3D Breast Cancer Detection

A comprehensive deep learning project implementing and comparing various neural network architectures for breast cancer detection in Digital Breast Tomosynthesis (DBT) scans.

## Authors
- **Olmo Ceriotti** (2193258)
- **Cristian Apostol** (2002291)

## Project Overview

This project develops and evaluates deep learning pipelines for detecting breast cancer in 3D DBT scans. The core implementation compares modern Vision Transformer architectures (specifically Swin Transformer) against traditional CNN baselines (ResNet-101), with an innovative extension using Parameterized Hypercomplex Neural Networks (PHNNs) for modeling inter-view correlations.

### Key Features

- **Multiple Architecture Implementations:**
  - ResNet3D Classifier (CNN baseline)
  - Swin3D Classifier (Vision Transformer)
  - Multi-view variants with attention mechanisms
  - HypercomplexDBT Classifier (novel PHNN approach)

- **Advanced Training Strategies:**
  - Self-supervised pre-training on DBT data
  - SIFT-DBT inspired fine-tuning methodology
  - F1-score optimized training for imbalanced datasets
  - Discriminative learning rates

- **Comprehensive Evaluation:**
  - Model performance comparison
  - Anomaly detection approaches
  - Grad-CAM interpretability analysis

## Dataset

The project utilizes the publicly available **Breast Cancer Screening-DBT (BCS-DBT)** dataset from The Cancer Imaging Archive (TCIA), ensuring reproducibility and fair comparison across architectures.

## Technical Implementation

### Core Architectures

1. **ResNet3DClassifier**: Hybrid CNN-Transformer using ResNet-101 for feature extraction and Transformer encoder for temporal aggregation
2. **Swin3DClassifier**: Vision Transformer-based approach with hierarchical feature extraction and self-attention mechanisms
3. **HypercomplexDBTClassifier**: Novel architecture using hypercomplex algebra for slice-wise multi-view fusion

### Key Features

- **Slice-wise Multi-view Fusion**: Integration of four anatomical views (RCC, RMLO, LCC, LMLO) at each slice depth
- **Hypercomplex Neural Networks**: Leveraging algebraic biases for structured multi-view correlation modeling
- **Advanced Fine-tuning**: DBT-specific pre-training with discriminative learning rates

## Files Structure

- `Notebook.ipynb`: Complete implementation with all models, training loops, and evaluation metrics
- `Neural Networks.pdf`: Detailed project documentation and theoretical background
- `README.md`: Project overview and setup instructions

---

*This project was completed as part of a Neural Networks course, focusing on advanced deep learning applications in medical imaging.*