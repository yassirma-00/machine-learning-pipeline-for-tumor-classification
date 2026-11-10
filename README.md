# complete-machine-learning-pipeline-for-tumor-classification

##  Installation

Clone the repository and install the required dependencies:

```bash
git clone https://github.com/your-username/breast-cancer-classification.git
cd breast-cancer-classification
pip install -r requirements.txt
```

---

##  Usage

### Run the Full Pipeline

```bash
python src/main.py
```

### Launch the Exploratory Analysis Notebook

```bash
jupyter notebook notebooks/exploration.ipynb
```

---

##  Dataset

This project uses the Breast Cancer Wisconsin dataset provided by Scikit-Learn.

| Feature | Value |
|----------|---------|
| Source | `sklearn.datasets.load_breast_cancer` |
| Samples | 569 |
| Features | 30 numerical features |
| Classes | Benign (357) / Malignant (212) |

---

##  Project Objectives

- Build a robust preprocessing pipeline using Scikit-Learn.
- Compare multiple machine learning algorithms.
- Optimize hyperparameters using automated search techniques.
- Evaluate model performance using stratified cross-validation.
- Interpret model predictions with SHAP.
- Save and export the best-performing model.

---

##  Machine Learning Models

###  Random Forest
An ensemble learning method based on multiple decision trees.

###  XGBoost
A powerful gradient boosting algorithm optimized for tabular data.
###  Support Vector Machine (SVM)
A classification algorithm that maximizes the margin between classes.

###  Multi-Layer Perceptron (MLP)
An artificial neural network designed for classification tasks.

---

##  Hyperparameter Optimization

Model hyperparameters are optimized using:

```python
RandomizedSearchCV
```

Features:

- Stratified 5-Fold Cross-Validation
- Randomized Hyperparameter Search
- Improved Model Generalization

---

## Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- Confusion Matrix
- Learning Curves

---

##  Model Interpretability

The project incorporates SHAP (SHapley Additive exPlanations) to:

- Explain model predictions.
- Identify the most influential features.
- Improve transparency and trust in the model.

---

##  Model Export

The best-performing model is automatically saved for future use:

```python
joblib.dump(best_model, "models/best_model.pkl")
```

---

    Courbes d'apprentissage
