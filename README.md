# Day 6: K-Nearest Neighbors (KNN) Classifier – Iris Dataset 🌸

---

## 🎯 Objective
Explore the K-Nearest Neighbors algorithm for classification on the classic Iris dataset. Focus areas include model evaluation, hyperparameter tuning, and decision boundary visualization using dimensionality reduction.

---

## 📁 Dataset
- **Source**: `sklearn.datasets.load_iris()`
- **Samples**: 150
- **Classes**: 3 (Setosa, Versicolor, Virginica)
- **Features**: Sepal & Petal measurements (4 features)
- **Missing values**: None

---

## 🧠 Core Concepts Covered
- Distance-based classification (KNN)
- Euclidean distance, majority voting
- Feature scaling (StandardScaler)
- Bias-variance tradeoff
- Hyperparameter tuning for `k`
- 2D visualization using PCA
- Decision boundary interpretation

---

## 🔧 Tools & Libraries
- Python
- scikit-learn
- matplotlib, seaborn
- PCA for 2D dimensionality reduction

---

## 📊 Model Performance (K = 5)

| Metric        | Value  |
|---------------|--------|
| Accuracy      | 93.33% |
| Precision     | ~94%   |
| Recall        | ~93%   |
| F1-score      | ~93%   |

Confusion Matrix showed strong performance across all 3 classes.

---

## 📈 K Value Tuning

Tested `k` values from 1 to 20.  
Observed best performance at:

- **K = 1, 7, 9+ → Accuracy ~96.7%**
- **K = 5 (default) → Accuracy ~93.3%**

Result: Model is **stable** across a wide range of `k`.

---

## 🌐 Decision Boundary

- Visualized using **PCA-reduced 2D features**
- Plotted classification regions and class boundaries
- Color-coded predictions and class distribution

---


---

## 🧠 Key Learnings

- KNN is a **lazy, non-parametric** model
- Performance depends heavily on **feature scaling** and **K selection**
- Visualization helps understand decision regions
- Simple yet powerful for small, well-separated datasets

---

## 🚀 Run the Project

```bash
# Clone the repo
git clone https://github.com/your-username/knn-iris-day6.git

cd knn-iris-day6

# (Optional) Create virtual environment
python -m venv venv
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook


