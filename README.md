#Palmer Penguins Species Classification

A supervised machine learning project that classifies penguin species — **Adelie**, **Chinstrap**, and **Gentoo** — from physical body measurements, comparing k-Nearest Neighbors and Decision Tree classifiers.

## Overview

This project builds and evaluates two classification models on the Palmer Penguins dataset to determine which approach most accurately predicts penguin species from morphological features. It was developed as a capstone project for a Python & Machine Learning workshop at the University of Dhaka.

## Dataset

| | |
|---|---|
| **Source** | `seaborn.load_dataset('penguins')` |
| **Raw size** | 344 rows × 7 columns |
| **Clean size** | 333 rows (11 rows with missing values dropped) |
| **Features** | `bill_length_mm`, `bill_depth_mm`, `flipper_length_mm`, `body_mass_g` |
| **Target** | `species` (Adelie, Chinstrap, Gentoo) |

## Methodology

1. **Data cleaning** — removed rows with missing values
2. **Exploratory analysis** — visualized feature distributions and species separability
3. **Model training** — trained k-NN and Decision Tree classifiers on a train/test split
4. **Evaluation** — compared accuracy and inspected feature importance

## Results

| Model | Accuracy |
|---|---|
| k-Nearest Neighbors (k=5) | ~82% |
| **Decision Tree** | **~98%** |

**Best model: Decision Tree**, which correctly classified nearly all test-set observations.

### Key Findings

- The Decision Tree achieved near-perfect classification on the held-out test set.
- **Flipper length** emerged as the single strongest predictor of species.
- k-NN performed respectably (~82%) even without feature scaling, though it lagged behind the Decision Tree.

## Project Structure

```
palmer-penguins-classification/
├── Project.ipynb    # Full analysis: data prep, EDA, modeling, evaluation
└── README.md
```

## Getting Started

1. Open [Google Colab](https://colab.research.google.com)
2. Upload `Project.ipynb`
3. Run **Runtime → Run all**

No installation required — `pandas`, `seaborn`, `scikit-learn`, and `matplotlib` are pre-installed in Colab.

## Tech Stack

- **pandas** — data loading and cleaning
- **seaborn** — dataset access and visualization
- **scikit-learn** — model training and evaluation
- **matplotlib** — charting

## Author

Saifur Rahman Antor — BSc Applied Mathematics, University of Dhaka
[GitHub](https://github.com/saifurrahmanantor)
