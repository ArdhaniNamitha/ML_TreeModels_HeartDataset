# ML_TreeModels_HeartDataset

A machine learning project using **Decision Tree** and **Random Forest** classifiers to predict heart disease. The project includes preprocessing, model training, evaluation, visualization of overfitting, feature importances, and decision tree structure.

---

##  Objective

The goal is to build interpretable and accurate models that predict whether a patient has heart disease based on clinical features. By analyzing model depth, feature importances, and performance metrics, this project demonstrates how tree-based methods can be applied to healthcare classification problems.

---

##  Dataset Description

The dataset contains **303 patient records** with **13 clinical features** such as age, sex, chest pain type, cholesterol level, maximum heart rate, and more.

- **Target Variable**: `target`  
  - `1` → presence of heart disease  
  - `0` → absence of heart disease  

**Download Dataset**: [Click to view/download the dataset](heart.csv)

---

##  Files Included

| File Name                  | Description                                                          |
|----------------------------|-----------------------------------------------------------------------|
| `code(Task5).ipynb`        | Google Colab notebook with all model code, training steps, and outputs|
| `heart.csv`                | Dataset used for training and testing                                 |
| `decision tree.png`        | Visualization of the trained decision tree                            |
| `feature Importances.png`  | Feature importance graph showing top predictive features              |
| `overfitting analysis.png` | Accuracy vs. depth graph to analyze model overfitting                 |
| `README.md`                | This project overview and instructions                                |



**View Decision Tree Plot**: [Decision Tree](decision%20tree.png)  
**View Feature Importances**: [Feature Importances](feature%20Importances.png)  
**View Overfitting Plot**: [Overfitting Analysis](overfitting%20analysis.png)

---

##  Steps Covered in the Project

### 1. Data Preprocessing
- Loaded `heart.csv` using pandas  
- Checked for missing values (none found)  
- Split into training and test sets using `train_test_split`

### 2. Decision Tree Classifier
- Trained a basic `DecisionTreeClassifier`  
- Evaluated accuracy and checked for overfitting  
- Visualized decision tree using `plot_tree` and saved as image  
- Controlled depth using `max_depth` to reduce overfitting

### 3. Overfitting Analysis
- Trained trees with varying depths  
- Plotted test accuracy vs. tree depth  
- Analyzed at what depth performance stabilized

### 4. Random Forest Classifier
- Trained `RandomForestClassifier`  
- Compared performance with Decision Tree  
- Evaluated using accuracy and confusion matrix

### 5. Feature Importance
- Extracted feature importances from Random Forest  
- Plotted top contributing features to heart disease prediction

---

##  Key Takeaways
- Decision Trees are intuitive but can easily overfit
- Random Forests are more accurate and stable
- Tree depth should be controlled to prevent overfitting
- Feature importance helps identify critical health indicators

---

##  How to Run

1. Open [Google Colab](https://colab.research.google.com/)
2. Upload the notebook: `code(Task5).ipynb`
3. Upload the dataset: `heart.csv`
4. Run each cell in order to see training, plots, and evaluation
5. PNGs will be generated automatically if `savefig()` is used in code

---

##  Future Enhancements
- Add hyperparameter tuning using GridSearchCV
- Introduce cross-validation for reliable evaluation
- Compare with additional models like XGBoost or LightGBM
- Create a simple Streamlit dashboard for predictions

---
