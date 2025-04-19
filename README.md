# 🧠 PARAMETER OPTIMIZATION of SVM on UCI DATASET

This repository contains code and analysis for optimizing a Support Vector Machine (SVM) on a UCI dataset.

## 🚀 Objective

- Use a dataset with **5k–30k rows**
- Split into **70-30 train-test ratio**, repeated over **10 samples**
- Run **100 iterations per sample** with different hyperparameters
- Track and save **best accuracy and SVM parameters** per sample
- Plot the **convergence graph** of the best-performing sample

## 🗂 Dataset Used

Used `Breast Cancer Dataset` from `sklearn.datasets` (you may replace with a UCI dataset).

## ⚙️ SVM Parameters Explored

- Kernels: `linear`, `rbf`, `poly`
- C: Random values from log scale [1e-3, 1e3]
- Gamma: Auto / log range

## 📦 Libraries Used

- `pandas`, `numpy`, `scikit-learn`
- `matplotlib` for plotting
- `tqdm` for progress bars

## 📊 Output

- **Table 1:** Comparative performance of Optimized-SVM with different samples
- **Figure 1:** Convergence graph showing how accuracy improved with iterations


## 📊 Results Table (Table 1):

| Sample | Best Accuracy | Best SVM Parameters (Kernel, C, Gamma)       |
|--------|----------------|----------------------------------------------|
| S1     | 0.982          | linear, 0.464, 0.005                         |
| S2     | 0.971          | rbf, 0.464, 0.022                            |
| S3     | 0.994          | linear, 0.1, 0.022                           |
| S4     | 0.988          | linear, 2.154, 46.416                        |
| S5     | 0.994          | rbf, 10.0, 0.005                             |
| S6     | 0.988          | linear, 0.022, 0.001                         |
| S7     | 0.982          | linear, 2.154, 0.001                         |
| S8     | 0.982          | linear, 0.464, 0.1                           |
| S9     | 0.988          | poly, 215.443, 0.022                         |
| S10    | 0.994          | linear, 2.154, 0.022                         |


## 📈 Convergence Graph

Shows iteration-wise accuracy for the best SVM sample.

![Convergence Graph of Best SVM](/content/convergence_graph.png)

## 💻 How to Run

1. Clone the repo or open the notebook in Google Colab.
2. Install dependencies (if needed).
3. Run all cells.
4. View results + convergence graph.

## 📝 Author

**BHAVYA**

