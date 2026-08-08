# 🍷 Wine Quality Prediction

## 📌 Project Overview

This project focuses on predicting the quality of red wine using Machine Learning classification algorithms. The prediction is based on various physicochemical properties such as acidity, alcohol content, density, pH, sulphates, and chlorides.

The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and comparison of multiple machine learning algorithms.

---

## 🎯 Objective

To build and compare multiple machine learning classification models that predict whether a wine is of **Good** or **Bad** quality based on its physicochemical characteristics.

---

## 📂 Dataset

- **Dataset:** Wine Quality (Red Wine)
- **Source:** UCI Machine Learning Repository
- **Samples:** 1,599
- **Features:** 11 Physicochemical Features
- **Target Variable:** Quality

### Features

- Fixed Acidity
- Volatile Acidity
- Citric Acid
- Residual Sugar
- Chlorides
- Free Sulfur Dioxide
- Total Sulfur Dioxide
- Density
- pH
- Sulphates
- Alcohol

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📊 Project Workflow

1. Import Libraries
2. Load Dataset
3. Data Inspection
4. Data Cleaning
5. Exploratory Data Analysis (EDA)
6. Class Imbalance Analysis
7. Feature Engineering
8. Data Preprocessing
9. Model Training
10. Model Evaluation
11. Feature Importance Analysis
12. Model Comparison
13. Conclusion

---

## 📈 Exploratory Data Analysis

The following analyses were performed:

- Quality Score Distribution
- Distribution of Chemical Features
- Correlation Heatmap
- Outlier Detection using Boxplots
- Feature Relationship Analysis

---

## ⚙️ Machine Learning Models

The following classification models were implemented:

- 🌳 Random Forest Classifier
- ⚡ Stochastic Gradient Descent (SGD) Classifier
- 🎯 Support Vector Classifier (SVC)

---

## 📊 Model Performance

| Model | Accuracy |
|--------|---------:|
| Support Vector Classifier (SVC) | **75.37%** |
| Random Forest Classifier | **75.00%** |
| SGD Classifier | **72.43%** |

---

## 🌟 Feature Importance

Random Forest identified the following as the most important features:

- Alcohol
- Sulphates
- Volatile Acidity
- Total Sulfur Dioxide
- Density

These features contributed the most to predicting wine quality.

---

## 📌 Key Findings

- Most wines belong to quality scores **5** and **6**.
- The original dataset exhibited class imbalance.
- Quality scores were converted into binary classes:
  - **Bad Wine (0)**
  - **Good Wine (1)**
- Feature scaling improved the performance of SGD and SVC models.
- Support Vector Classifier achieved the highest prediction accuracy among the evaluated models.

---

## 🏆 Conclusion

This project successfully developed a machine learning-based wine quality prediction system using physicochemical properties of red wine.

Among the three evaluated models, the **Support Vector Classifier (SVC)** achieved the highest accuracy of **75.37%**, making it the most suitable model for this dataset.

The project demonstrates the complete machine learning workflow, including data preprocessing, exploratory data analysis, feature engineering, model training, evaluation, and performance comparison.

---

## 📁 Project Structure

```
DataAnalytics-L2-WineQualityPrediction/
│
├── data/
│   └── WineQuality-RedWine.csv
│
├── notebook/
│   └── Wine_Quality_Prediction.ipynb
│
├── README.md
└── requirements.txt
```

---

## 📚 Future Improvements

- Hyperparameter tuning using GridSearchCV
- Cross-validation for more robust evaluation
- Multi-class classification instead of binary classification
- Deployment using Flask or Streamlit
- Model explainability using SHAP or LIME

---

## 👨‍💻 Author

**Vamshi Yadav Kodi**

B.Tech – Computer Science Engineering

Oasis Infobyte Data Analytics Internship
