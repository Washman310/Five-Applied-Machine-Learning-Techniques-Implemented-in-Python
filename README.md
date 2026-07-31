# Five Applied Machine Learning Techniques Implemented in Python

![Python](https://img.shields.io/badge/Python-3.11-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)
![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-yellow)
![License](https://img.shields.io/badge/License-MIT-green)

## Overview

This project demonstrates the implementation of five modern machine learning workflows using real-world datasets and widely adopted Python libraries. Each workflow highlights a different area of applied machine learning, ranging from transformer-based natural language processing to explainable artificial intelligence.

The objective of the project is to demonstrate the complete machine learning lifecycle:

- Data preprocessing
- Feature engineering
- Model development
- Hyperparameter optimization
- Model evaluation
- Model interpretation
- Visualization of results

Although each workflow is independent, together they provide a broad overview of practical machine learning techniques commonly encountered in industry.

---

## Machine Learning Workflows

### 1. Transformer-Based Natural Language Processing

- Fine-tuned DistilBERT using the Hugging Face Transformers library
- Sentiment classification on the IMDB Movie Reviews dataset
- Performance evaluated using:
  - Accuracy
  - Precision
  - Recall
  - F1 Score

---

### 2. Evolutionary Hyperparameter Optimization

Applied evolutionary optimization techniques to improve machine learning model performance using the Wine Quality dataset.

Topics include:

- Evolution Strategies
- Hyperparameter Optimization
- Performance Comparison
- Convergence Analysis

---

### 3. Decision Tree Classification

Implemented and optimized a Decision Tree classifier using the Titanic Survival dataset.

Included:

- Hyperparameter tuning
- Cross-validation
- Feature importance analysis
- Decision tree visualization

---

### 4. Hybrid Ensemble Learning

Developed multiple specialized machine learning models for web page classification using the Evergreen Classification dataset.

Techniques include:

- TF-IDF
- Ensemble learning
- Majority voting
- Specialized feature models

---

### 5. Explainable Artificial Intelligence

Built a heart disease prediction model and interpreted predictions using Local Interpretable Model-Agnostic Explanations (LIME).

This workflow demonstrates how modern machine learning models can be made more transparent and interpretable.

---

# Repository Structure

```
Five-Applied-Machine-Learning-Techniques-Implemented-in-Python/

├── images/
├── notebooks/
├── data/
├── outputs/
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

# Technologies Used

Programming

- Python

Machine Learning

- scikit-learn
- Hugging Face Transformers
- LIME

Data Processing

- pandas
- NumPy
- SciPy

Visualization

- matplotlib
- seaborn

Optimization

- Evolution Strategies

Development Environment

- Jupyter Notebook

---

# Installation

## 1. Clone the repository

```bash
git clone https://github.com/Washman310/Five-Applied-Machine-Learning-Techniques-Implemented-in-Python.git

cd Five-Applied-Machine-Learning-Techniques-Implemented-in-Python
```

---

## 2. Create a virtual environment (recommended)

Windows

```bash
python -m venv .venv

.venv\Scripts\activate
```

Linux / macOS

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

## 4. Download datasets

The IMDB Movie Reviews dataset is not included in this repository due to file size.

Download:

IMDB Dataset of 50K Movie Reviews

Place the downloaded file here:

```
data/imdb/IMDB Dataset.csv
```

All remaining datasets are already included.

---

## 5. Launch Jupyter

```bash
jupyter notebook
```

Open

```
notebooks/applied_machine_learning_workflows.ipynb
```

Run the notebook sequentially from top to bottom.

---

# Results

The notebook generates:

- Performance metrics
- Confusion matrices
- Decision tree visualizations
- LIME explanations
- BERT predictions
- Ensemble learning comparisons

Representative figures are provided in the **images/** directory.

---

# Images

The repository includes representative visualizations generated during model training and evaluation.

Examples include:

- Architecture Diagram
- Confusion Matrix
- Decision Tree Visualization
- LIME Explanation
- BERT Prediction Example
- Evolution Strategy Convergence Plot

---

# Troubleshooting

## IMDB dataset not found

Verify that

```
data/imdb/IMDB Dataset.csv
```

exists.

---

## CUDA warnings

The notebook automatically falls back to CPU execution if CUDA is unavailable.

---

## ModuleNotFoundError

Run

```bash
pip install -r requirements.txt
```

again.

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
- Docker deployment

---

# Author

William Ashman

Operations Research & Systems Analyst

Johns Hopkins University — M.S. Data Science

---

# License

This project is licensed under the MIT License.
