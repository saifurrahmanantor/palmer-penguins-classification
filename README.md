# 🐧 Palmer Penguins Classification

A machine learning project that classifies penguin species — **Adelie**, **Chinstrap**, and **Gentoo** — based on physical measurements, built as a capstone project for a Python & Machine Learning workshop.

## 📌 Project Overview

The goal was to build and compare two classification models on the [Palmer Penguins dataset](https://github.com/allisonhorst/palmerpenguins) and evaluate which one performs better at predicting penguin species from body measurements.

## 📂 Dataset

- **Source:** `seaborn.load_dataset('penguins')`
- **344 rows**, 7 columns
- **Features used:** `bill_length_mm`, `bill_depth_mm`, `flipper_length_mm`, `body_mass_g`
- **Target:** `species` (Adelie, Chinstrap, Gentoo)
- **Preprocessing:** Dropped 11 rows with missing values → 333 clean rows

## 🔬 Models Trained

| Model | Accuracy |
|---|---|
| k-Nearest Neighbors (k=5) | ~82% |
| Decision Tree | 100% |

✅ **Winner: Decision Tree**

---

## 📊 Key Findings

- The **Decision Tree** perfectly classified all penguin species on the test set
- The most important feature was **flipper length** — the single strongest predictor of species
- **k-NN** still performed well at ~82% without any feature scaling

---

## 🗂️ Project Structure

```
palmer-penguins-classification/
│
├── Project.ipynb       # Main Jupyter Notebook (all 3 phases)
└── README.md
```

---

## 🚀 How to Run

1. Open [Google Colab](https://colab.research.google.com)
2. Upload `Project.ipynb`
3. Click **Runtime → Run all**

No extra installs needed — all libraries (`pandas`, `seaborn`, `scikit-learn`, `matplotlib`) are pre-installed in Colab.

---

## 🛠️ Libraries Used

- `pandas` — data loading and cleaning
- `seaborn` — dataset and visualisation
- `scikit-learn` — model training and evaluation
- `matplotlib` — charts and plots

---

## 📧 Submission

Project submitted as part of the Machine Learning Capstone at **University of Dhaka**.
