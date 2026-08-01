# Five Applied Machine Learning Techniques Implemented in Python

![Python](https://img.shields.io/badge/Python-3.12-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)
![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-yellow)
![License](https://img.shields.io/badge/License-MIT-green)

## Overview

This project demonstrates the implementation of five modern machine learning workflows using real-world datasets and widely adopted Python libraries. Each workflow highlights a different area of applied machine learning, ranging from transformer-based natural language processing to explainable artificial intelligence.

The objective of this project is to demonstrate the complete machine learning lifecycle, including:

- Data preprocessing
- Feature engineering
- Model development
- Hyperparameter optimization
- Model evaluation
- Model interpretation
- Visualization of results

Although each workflow is independent, together they provide a broad overview of practical machine learning techniques commonly encountered in industry.

---

# Machine Learning Workflows

## 1. Transformer-Based Natural Language Processing

- Fine-tuned DistilBERT using the Hugging Face Transformers library
- Sentiment classification on the IMDB Movie Reviews dataset
- GPU acceleration when CUDA is available
- Performance evaluated using:
  - Accuracy
  - Precision
  - Recall
  - F1 Score

---

## 2. Evolutionary Hyperparameter Optimization

Applied evolutionary optimization techniques to improve machine learning model performance using the Wine Quality dataset.

Topics include:

- Evolution Strategies
- Hyperparameter Optimization
- Performance Comparison
- Convergence Analysis

---

## 3. Decision Tree Classification

Implemented and optimized a Decision Tree classifier using the Titanic Survival dataset.

Included:

- Hyperparameter tuning
- Cross-validation
- Feature importance analysis
- Decision tree visualization

---

## 4. Hybrid Ensemble Learning

Developed multiple specialized machine learning models for web page classification using the Evergreen Classification dataset.

Techniques include:

- TF-IDF
- Random Forest
- Support Vector Machines
- Ensemble learning
- Majority voting
- Specialized feature models

---

## 5. Explainable Artificial Intelligence

Built a heart disease prediction model and interpreted predictions using Local Interpretable Model-Agnostic Explanations (LIME).

This workflow demonstrates how modern machine learning models can be made more transparent and interpretable.

---

# Repository Structure

```
Five-Applied-Machine-Learning-Techniques-Implemented-in-Python/

├── data/
│   ├── imdb/
│   ├── wine_quality/
│   ├── titanic/
│   ├── evergreen/
│   └── heart_disease/
│
├── images/
├── notebooks/
├── outputs/
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

# Technologies Used

### Programming

- Python

### Machine Learning

- scikit-learn
- Hugging Face Transformers
- LIME

### Data Processing

- pandas
- NumPy
- SciPy

### Visualization

- matplotlib

### Optimization

- Evolution Strategies

### Development Environment

- Jupyter Notebook

---

# Installation

## 1. Clone the repository

```bash
git clone https://github.com/Washman310/Five-Applied-Machine-Learning-Techniques-Implemented-in-Python.git

cd Five-Applied-Machine-Learning-Techniques-Implemented-in-Python
```

---

## 2. (Recommended) Create a virtual environment

### Windows

```bash
python -m venv .venv

.venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv .venv

source .venv/bin/activate
```

---

## 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 4. Download the IMDB dataset

The IMDB Movie Reviews dataset is not included in this repository due to licensing and file size.

Download:

**IMDB Dataset of 50K Movie Reviews**

Place the downloaded file in:

```
data/imdb/IMDB Dataset.csv
```

All remaining datasets required by the notebook are included in the repository.

---

## 5. (Optional) Enable GPU Acceleration

The notebook automatically uses an NVIDIA GPU if CUDA-enabled PyTorch is installed.

Verify GPU availability:

```python
import torch

print(torch.cuda.is_available())

if torch.cuda.is_available():
    print(torch.cuda.get_device_name(0))
```

If `torch.cuda.is_available()` returns `False`, the notebook will automatically execute using the CPU.

GPU acceleration is recommended for the transformer-based NLP workflow and significantly reduces execution time.

---

## 6. Launch Jupyter

```bash
jupyter notebook
```

Open:

```
notebooks/Five Applied Machine Learning Techniques Implemented in Python.ipynb
```

Run the notebook sequentially from top to bottom.

The notebook automatically detects the cloned repository location and loads datasets from the repository's `data/` directory. No manual path configuration is required.

---

# Expected Runtime

Approximate execution time on modern hardware:

| Hardware | Approximate Runtime |
|-----------|--------------------:|
| NVIDIA GPU | 15–30 minutes |
| Modern CPU | 30–60 minutes |

Most of the runtime comes from the transformer-based natural language processing workflow.

---

# Results

Running the notebook produces:

- Performance metrics
- Confusion matrices
- Decision tree visualizations
- LIME explanations
- BERT sentiment predictions
- Ensemble learning comparisons
- Evolution Strategy convergence plots

Generated artifacts are written to the `outputs/` directory.

Representative figures are included in the `images/` directory.

---

# Images

Example visualizations include:

- Pipeline Architecture
- Confusion Matrix
- Decision Tree Visualization
- LIME Explanation
- DistilBERT Prediction Example
- Evolution Strategy Convergence Plot

---

# Troubleshooting

## IMDB dataset not found

Verify that:

```
data/imdb/IMDB Dataset.csv
```

exists.

---

## CUDA unavailable

The notebook automatically falls back to CPU execution when CUDA is unavailable.

To verify GPU detection:

```python
import torch

print(torch.cuda.is_available())
```

---

## ModuleNotFoundError

Reinstall the project dependencies:

```bash
pip install -r requirements.txt
```

---

## Notebook kernel crashes

Restart the kernel and execute the notebook from the first cell.

---

# Future Improvements

Potential extensions include:

- SHAP explanations
- Optuna hyperparameter optimization
- XGBoost implementation
- Transformer model comparison
- Deep neural networks
- MLflow experiment tracking
- Docker containerization

---

# Author

**William Ashman**

Operations Research & Systems Analyst

Johns Hopkins University  
M.S. Data Science

---

# License

This project is licensed under the MIT License.