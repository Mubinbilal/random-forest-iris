# random-forest-iris
Random Forest Classifier on the Iris dataset — includes ensemble training, n_estimators hyperparameter tuning (20/50/100/200), confusion matrix evaluation, and feature importance visualization.
# 🌲🌲 Random Forest Classifier on Iris Dataset

A beginner-to-intermediate implementation of a **Random Forest Classifier** using Python and Scikit-learn. This project trains an ensemble model on the Iris dataset, tunes the number of trees, evaluates performance, and visualizes feature importances.

---

## 🔍 Overview

This notebook walks through a complete Random Forest classification workflow:

1. **Load** the Iris dataset and inspect class/feature names
2. **Split** data into training and test sets (75/25, stratified)
3. **Train** a Random Forest with 100 decision trees
4. **Evaluate** performance with accuracy score and confusion matrix
5. **Tune** the model by comparing different `n_estimators` values (20, 50, 100, 200)
6. **Visualize** feature importances with a horizontal bar chart

---

## 📁 Project Structure

```
random-forest-iris/
│
├── Random_forest_implementation_.ipynb   # Main Jupyter Notebook
└── README.md                             # Project documentation
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3 | Core language |
| NumPy | Array operations and sorting |
| Scikit-learn | Dataset, model training & evaluation |
| Matplotlib | Feature importance visualization |
| Jupyter Notebook | Interactive development environment |

---

## 📊 Dataset — Iris

The built-in **Iris dataset** from Scikit-learn — 150 samples, 3 classes, 4 features:

| Feature | Description |
|---|---|
| Sepal length | Length of the sepal (cm) |
| Sepal width | Width of the sepal (cm) |
| Petal length | Length of the petal (cm) |
| Petal width | Width of the petal (cm) |

**Classes:** Setosa, Versicolor, Virginica

---

## ⚙️ Model Configuration

```python
RandomForestClassifier(
    n_estimators=100,
    max_depth=None,
    random_state=42
)
```

- **`n_estimators=100`** — builds an ensemble of 100 decision trees
- **`max_depth=None`** — trees grow fully until all leaves are pure
- **`stratify=y`** — preserves class balance in the train/test split

---

## 🔧 Hyperparameter Tuning

The notebook compares four values of `n_estimators` to find the best performing model:

| n_estimators | Notes |
|---|---|
| 20 | Fewer trees, faster training |
| 50 | Balanced speed and accuracy |
| 100 | Default — strong baseline |
| 200 | More trees, diminishing returns |

The best `n_estimators` is automatically selected based on test accuracy.

---

## 📈 Evaluation Metrics

- **Accuracy Score** — overall percentage of correct predictions
- **Confusion Matrix** — true vs. predicted labels per class
- **Feature Importances** — bar chart showing which features drive predictions most

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/random-forest-iris.git
cd random-forest-iris
```

### 2. Install dependencies

```bash
pip install numpy scikit-learn matplotlib notebook
```

### 3. Launch the notebook

```bash
jupyter notebook Random_forest_implementation_.ipynb
```

---

## 💡 Key Concepts Covered

- What is a Random Forest and how it differs from a single Decision Tree
- Ensemble learning via bagging
- Stratified train/test splitting
- Hyperparameter tuning with `n_estimators`
- Feature importance extraction and visualization

---

## 🙌 Acknowledgements

Built as a learning project to understand ensemble methods and the power of combining multiple decision trees using the Scikit-learn library.
