# Heart_tree_Models_Analysis
This project uses tree-based machine learning models to predict the presence of heart disease based on various medical attributes. It includes Decision Tree and Random Forest classifiers, with evaluation and interpretability analysis.

## 📁 Dataset
- **File**: `heart.csv`
- **Rows**: 1025
- **Target Variable**: `target` (0 = No heart disease, 1 = Heart disease)
- **Features**: `age`, `sex`, `cp`, `trestbps`, `chol`, `fbs`, `restecg`, `thalach`, `exang`, `oldpeak`, `slope`, `ca`, `thal`

## 🎯 Objective
- Train a **Decision Tree Classifier** and visualize the tree  
- Analyze **overfitting** and control **tree depth**  
- Train a **Random Forest Classifier** and compare its performance  
- Analyze **feature importances**  
- Evaluate models using **cross-validation**

## 📊 Exploratory Data Analysis
- Strong correlations with heart disease:
  - Positive: `cp`, `thalach`, `slope`
  - Negative: `exang`, `oldpeak`, `ca`, `thal`
- Weak correlations: `age`, `chol`, `fbs`

## 🌳 Models and Performance

### ✅ Decision Tree
- Trained and visualized
- **Overfitting** observed at higher depths
- Depth tuning helps balance bias and variance

### 🌲 Random Forest
- Achieved higher accuracy
- More robust to overfitting

### 📈 Accuracy (Sample Output)

| Model            | Accuracy | CV Accuracy |
|------------------|----------|-------------|
| Decision Tree    | ~79%     | ~76%        |
| Random Forest    | ~84%     | ~82%        |

## 🧠 Feature Importance (Top 5)
1. `cp` (chest pain type)  
2. `ca` (number of major vessels)  
3. `thalach` (maximum heart rate)  
4. `oldpeak` (ST depression)  
5. `thal` (thalassemia)


## 🔁 Cross-Validation
- 5-fold cross-validation used  
- Random Forest had better generalization

## 📌 Conclusion
Tree-based models are effective in medical diagnosis tasks. Random Forest outperformed Decision Tree in terms of both accuracy and stability. Feature importance analysis provides clinical interpretability of model decisions.

## 🛠️ Libraries Used
- `pandas`, `numpy`, `seaborn`, `matplotlib`
- `scikit-learn`.
