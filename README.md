# MNIST Classifiers & California Housing Regressors

This project is a **Deep Learning** initiative designed as a **review of core Machine Learning concepts**. It focuses on two classic datasets:

- **Classification using the MNIST dataset**
- **Regression using the California Housing dataset**

Our goal was to apply traditional ML models and perform **hyperparameter tuning using Grid Search** with **3-fold cross-validation (CV)** to find the best configuration for each model.

---

## 🔢 Classification - MNIST

The MNIST dataset was used to train and compare different classifiers. The evaluation metric was **mean accuracy** during cross-validation.

### ✅ Best Models and Results:

- **Decision Tree Classifier**
  - Hyperparameters: `criterion='entropy'`, `max_depth=20`, `min_samples_leaf=1`, `min_samples_split=2`
  - Best accuracy: **0.8594**

- **Support Vector Classifier (SVC)**
  - Hyperparameters: `C=10`, `gamma=0.001`, `kernel='rbf'`
  - Best accuracy: **0.9889**

- **Logistic Regression**
  - Hyperparameters: `C=1`, `penalty='l1'`, `solver='liblinear'`, `max_iter=1000`, `n_jobs=-1`
  - Best accuracy: **0.9582**

---

## 🏠 Regression - California Housing

The California Housing dataset was used for training regression models. The evaluation metric was the **negative Mean Squared Error (MSE)** (as used by `GridSearchCV`).

### 📊 Best Models and Results:

- **Decision Tree Regressor**
  - Hyperparameters: `max_depth=10`, `min_samples_leaf=4`, `min_samples_split=10`, `random_state=42`
  - Best MSE: **-0.4152**

- **Support Vector Regressor (SVR)**
  - Hyperparameters: `C=1`, `epsilon=1`, `kernel='rbf'`, `max_iter=500`
  - Best MSE: **-0.4593**

- **Linear Regression**
  - Hyperparameters: `copy_X=True`, `fit_intercept=True`, `n_jobs=-1`, `positive=False`
  - Best MSE: **-0.5199**

---

## 🛠 Tools and Technologies

- Python
- Scikit-learn
- GridSearchCV
- Jupyter Notebooks (for experimentation)

---

## 📚 Educational Purpose

This project aims to reinforce understanding of:

- Data preprocessing
- Training and validating supervised models
- Hyperparameter optimization
- Interpreting evaluation metrics

---

Feel free to explore the notebooks and modify the experiments for your own learning!
