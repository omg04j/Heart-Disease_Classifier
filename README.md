# Heart Disease Classification Project

## 📋 Overview
This project implements multiple machine learning models to predict the presence of heart disease based on various medical attributes. After comparing different algorithms, Logistic Regression emerged as the best performing model. The project aims to assist medical professionals in early detection and risk assessment of heart disease.

## 🎯 Features
- Binary classification of heart disease presence (1 = yes, 0 = no)
- Comparison of multiple classification algorithms:
  - K-Nearest Neighbors (KNN)
  - Random Forest
  - Logistic Regression
- Data preprocessing and feature engineering
- Model performance comparison
- Performance metrics visualization

## 🔧 Technologies Used
- Python 3.x
- Libraries:
  - scikit-learn (for KNN, Random Forest, and Logistic Regression)
  - pandas (for data manipulation)
  - numpy (for numerical operations)
  - matplotlib (for visualization)
  - seaborn (for enhanced visualizations)

## 📊 Dataset
The project uses the Cleveland Heart Disease dataset from the UCI Machine Learning Repository.

### Data Sources
- Original dataset: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/heart+Disease)
- Alternative source: [Kaggle](https://www.kaggle.com/datasets/sumaiyatasmeem/heart-disease-classification-dataset)

### Data Dictionary
1. **age** - Age in years
2. **sex** - Gender (1 = male; 0 = female)
3. **cp** - Chest pain type
   * 0: Typical angina (heart-related chest pain)
   * 1: Atypical angina (non-heart-related chest pain)
   * 2: Non-anginal pain (typically esophageal spasms)
   * 3: Asymptomatic (no signs of disease)
4. **trestbps** - Resting blood pressure in mm Hg (>130-140 indicates concern)
5. **chol** - Serum cholesterol in mg/dl
   * Calculated as: LDL + HDL + 0.2 * triglycerides
   * Values >200 indicate concern
6. **fbs** - Fasting blood sugar >120 mg/dl (1 = true; 0 = false)
   * >126 mg/dL signals diabetes
7. **restecg** - Resting electrocardiographic results
   * 0: Normal
   * 1: ST-T Wave abnormality (from mild to severe)
   * 2: Probable/definite left ventricular hypertrophy
8. **thalach** - Maximum heart rate achieved
9. **exang** - Exercise-induced angina (1 = yes; 0 = no)
10. **oldpeak** - ST depression induced by exercise relative to rest
11. **slope** - Peak exercise ST segment slope
    * 0: Upsloping (better heart rate with exercise, uncommon)
    * 1: Flatsloping (minimal change, typical healthy heart)
    * 2: Downsloping (signs of unhealthy heart)
12. **ca** - Number of major vessels colored by fluoroscopy (0-3)
13. **thal** - Thallium stress test result
    * 1,3: Normal
    * 6: Fixed defect (previous defect, now ok)
    * 7: Reversible defect (improper blood flow during exercise)
14. **target** - Heart disease presence (1 = yes, 0 = no)

## Model Performance and Evaluation
- Performed hyperparameter tuning using:
  - RandomizedSearchCV for initial parameter space exploration
  - GridSearchCV for fine-tuning
  -  k-fold (k=5) cross-validation for robust evaluation 

## 📈 Model Performance Metrices
The project implements three different classification models with the following performance metrics:

### 1. Logistic Regression (Best Performing Model)
- Accuracy: 84.47%
- Precision: 82.08%
- Recall: 92.12%
- F1-Score: 86.73%
- AUC Score: 0.93
- ROC curve analysis performed for model evaluation


### 2. Random Forest
- Accuracy: 80.33%

### 3. K-Nearest Neighbors (KNN)
- Accuracy: 75.41%

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## 👥 Contact
- **Om Prakash Gadhwal**
- GitHub: [link](https://github.com/omg04j)
- LinkedIn: [link](in/omprakash-gadhwal-19422628b)

## 🙏 Acknowledgments
- UCI Machine Learning Repository for providing the Cleveland Heart Disease dataset
- The medical professionals who collected and annotated the original data
- The Kaggle community for maintaining an accessible version of the dataset
