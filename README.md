# Week 5: Ensemble Methods & Advanced Algorithms

## 📁 Project Structure

```
week5/
├── random_forest.py
├── xgboost_implementation.py
├── svm_classification.py
└── model_evaluation.py
```

---

## 🗂️ Tasks Overview

| Task | File | Algorithm |
|------|------|-----------|
| 5.1 | `random_forest.py` | Random Forest Classifier
| 5.2 | `xgboost_implementation.py` | Gradient Boosting (XGBoost) 
| 5.3 | `svm_classification.py` | Support Vector Machines 
| 5.4 | `model_evaluation.py` | Cross-Validation & Evaluation 

---

## 📌 Task Details

### Task 5.1 — Random Forest Classifier
Implements a Random Forest on a classification dataset (Heart Disease / Bank Marketing) with hyperparameter tuning via `GridSearchCV`.

**Key Features:**
- Experiments with `n_estimators` ∈ {10, 50, 100, 200} and `max_depth` ∈ {3, 5, 10, None}
- Comparison against a single Decision Tree
- Feature importance plot
- Out-of-Bag (OOB) error curve vs. number of estimators
- Best model saved to disk

---

### Task 5.2 — Gradient Boosting (XGBoost)
Implements XGBoost classifier with tuning and interpretability tools.

**Key Features:**
- GridSearchCV over `learning_rate`, `max_depth`, `n_estimators`
- Training history plotted using `eval_set`
- Feature importance visualization
- SHAP summary plot for model interpretability
- Model saved in both `.pkl` and `.json` formats
- Performance comparison with Random Forest



---

### Task 5.3 — Support Vector Machines (SVM)
Trains SVM classifiers with three different kernels on a 2D dataset and visualizes decision boundaries.

**Key Features:**
- Kernels: `linear`, `rbf`, `polynomial`
- Decision boundary plots for each kernel
- Hyperparameter sweep: `C` ∈ {0.1, 1, 10, 100}, `gamma` ∈ {0.001, 0.01, 0.1, 1}
- Accuracy vs. C and gamma plots
- Kernel comparison table
- Best model saved to disk

---

### Task 5.4 — Model Evaluation & Cross-Validation
Comprehensive model evaluation using multiple cross-validation strategies across three classifiers.

**Key Features:**
- k-Fold CV (k=5), Stratified k-Fold, and Leave-One-Out CV
- Models evaluated: Logistic Regression, Random Forest, SVM
- Mean ± std of CV scores (confidence intervals)
- Learning curves and validation curves per model
- Documented guidelines on when to use each evaluation strategy

---

---

## 📊 Techniques Used

| Technique | Purpose |
|-----------|---------|
| GridSearchCV | Hyperparameter tuning |
| OOB Error | Random Forest generalization estimate |
| SHAP Values | Model interpretability |
| Decision Boundaries | SVM kernel visualization |
| Learning Curves | Diagnosing bias/variance |
| Validation Curves | Hyperparameter impact analysis |
| Stratified K-Fold | Handling class imbalance in CV |
