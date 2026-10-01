# PyTorch Digit Classification

A systematic 5-stage deep learning project optimizing a Multi-Layer Perceptron (MLP) architecture in PyTorch for 32x32 grayscale handwritten digit classification, improving test accuracy from an 83.3% baseline to **87.6%**.

---

## 📌 Performance Summary

| Exp | Key Strategy | Configuration Highlights | Run Time | Test Accuracy |
| :-: | :--- | :--- | :-: | :-: |
| [**01**](./notebooks/01_baseline_architecture.ipynb) | Baseline Architecture | 1024-node Hidden Layer | 13.29 min | 83.3% |
| [**02**](./notebooks/02_scaling_model_capacity.ipynb) | Scaling Model Capacity | 2048-node Hidden Layer | 15.45 min | 83.5% |
| [**03**](./notebooks/03_increasing_training_time.ipynb) | Increasing Training Time | 2048-node + 80 Epochs | 29.36 min | 85.8% |
| [**04**](./notebooks/04_targeted_error_correction.ipynb) | Targeted Error Correction | Weighted Loss (Class 3) | 29.86 min | 87.2% |
| [**05**](./notebooks/05_refined_regularization.ipynb) | Refined Regularization | Reduced Dropout (0.2) | 31.79 min | **87.6%** |

*Note: Click on any experiment link above to inspect the corresponding Jupyter notebook, raw text log (`.txt`), and standardized convergence plots.*

---

## 📁 Repository Structure

```text
pytorch-digit-classification/
│
├── docs/                             # Final assignment report PDF
│   ├── .gitkeep
│   └── report.pdf
│
├── notebooks/                        # Notebooks, text logs, and standardized plots
│   ├── .gitkeep
│   ├── 01_baseline_architecture.ipynb
│   ├── 01_baseline_architecture_log.txt
│   ├── 01_baseline_architecture_standardized_plots.png
│   ├── 02_scaling_model_capacity.ipynb
│   ├── 02_scaling_model_capacity_log.txt
│   ├── 02_scaling_model_capacity_standardized_plots.png
│   ├── 03_increasing_training_time.ipynb
│   ├── 03_increasing_training_time_log.txt
│   ├── 03_increasing_training_time_standardized_plots.png
│   ├── 04_targeted_error_correction.ipynb
│   ├── 04_targeted_error_correction_log.txt
│   ├── 04_targeted_error_correction_standardized_plots.png
│   ├── 05_refined_regularization.ipynb
│   ├── 05_refined_regularization_log.txt
│   └── 05_refined_regularization_standardized_plots.png
│
├── .gitignore                        # Exclusion rules for checkpoints and dataset
├── requirements.txt                  # Python environment dependencies
└── README.md                         # Project documentation
```

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone [https://github.com/yourusername/pytorch-digit-classification.git](https://github.com/yourusername/pytorch-digit-classification.git)
cd pytorch-digit-classification
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Download the Dataset
1. Download `data.zip` from [GitHub Releases].
2. Extract the archive into a local `data/` directory in the project root:
```text
pytorch-digit-classification/
└── data/
    └── (extracted image subfolders)
```

### 4. Run the Notebooks
Launch Jupyter Notebook or JupyterLab to execute any experiment sequentially:
```bash
jupyter notebook notebooks/
```

---

## 📄 Final Written Report
For a complete theoretical analysis covering model selection, Batch Normalization, data augmentation, and class-wise error profiling, refer to the project report:
👉 [`docs/report.pdf`](./docs/report.pdf)
