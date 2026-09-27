#  Diabetes Risk Prediction & Healthcare Analytics

> An end-to-end Machine Learning project for analyzing healthcare indicators and predicting diabetes risk using Python and Scikit-learn.

##  Project Overview

Diabetes Risk Prediction & Healthcare Analytics is a Data Science and Machine Learning project that analyzes real-world healthcare indicators and develops classification models to identify diabetes risk.

The project follows a complete machine learning workflow — from data cleaning and exploratory data analysis to model development, evaluation, interpretability, error analysis, and final insights.

The main objective is to understand how different health and lifestyle indicators relate to diabetes risk and evaluate different Machine Learning algorithms on the classification problem.

##  Project Repository

GitHub:
https://github.com/rohanbhowm25308/Diabetes-Risk-Prediction-Healthcare-Analytics

## 🎯 Objectives

-  Clean and preprocess real-world healthcare data
-  Perform Exploratory Data Analysis (EDA)
-  Analyze important health and lifestyle indicators
-  Develop multiple Machine Learning classification models
-  Compare models using multiple evaluation metrics
-  Analyze prediction errors
-  Identify important features influencing predictions
-  Handle class imbalance
-  Analyze overfitting and underfitting
-  Visualize model performance
-  Generate meaningful healthcare analytics insights

##  Dataset

This project uses the Diabetes Health Indicators Dataset, based on the CDC's Behavioral Risk Factor Surveillance System (BRFSS).

### Dataset File

diabetes_binary_health_indicators_BRFSS2015.csv

### Dataset Information

| Property | Details |
|---|---|
| Dataset | Diabetes Health Indicators |
| Domain | Healthcare / Data Science |
| Problem Type | Binary Classification |
| Target Variable | Diabetes_binary |
| Records | 253,680 |
| Features | 21 |
| Programming Language | Python |
| ML Framework | Scikit-learn |

### Target Variable

- `0` → No diabetes
- `1` → Prediabetes or diabetes

>  This project is intended for educational and analytical purposes only and should not be used as a medical diagnostic system.

##  Machine Learning Workflow

Raw Healthcare Dataset
        ↓
Data Loading
        ↓
Data Inspection
        ↓
Data Cleaning
        ↓
Duplicate Removal
        ↓
Exploratory Data Analysis
        ↓
Feature Analysis
        ↓
Train-Test Split
        ↓
Data Preprocessing
        ↓
Model Training
        ↓
Model Evaluation
        ↓
Performance Comparison
        ↓
Error Analysis
        ↓
Feature Importance
        ↓
Final Insights

##  Machine Learning Models

### 1. Logistic Regression

Used as an interpretable baseline classification model.

- Simple and efficient
- Suitable for binary classification
- Provides probability estimates
- Easy to interpret

### 2. Decision Tree

A tree-based classification algorithm capable of learning nonlinear relationships.

- Easy to understand
- Captures nonlinear relationships
- Provides feature importance
- Does not require feature scaling

### 3. Random Forest

An ensemble learning algorithm that combines multiple decision trees.

- Handles nonlinear relationships
- Robust against noise
- Provides feature importance
- Can improve generalization compared with a single decision tree

##  Data Preprocessing

The project performs:

- Dataset loading
- Dataset structure inspection
- Missing-value analysis
- Duplicate detection
- Duplicate removal
- Target-variable analysis
- Feature and target separation
- Train-test splitting
- Feature scaling where required
- Class imbalance handling

For Logistic Regression, StandardScaler is used for feature scaling.

Class weighting is also considered to help address the imbalance between target classes.

##  Exploratory Data Analysis

The project performs detailed exploratory analysis to understand relationships within the healthcare data.

### Analysis Includes

- Target class distribution
- BMI analysis
- General health analysis
- Health indicators vs diabetes
- Feature correlations
- Target correlations
- Lifestyle indicators
- Distribution comparisons between target classes

### Visualizations

-  Target Distribution
-  BMI Analysis
-  General Health Analysis
-  Correlation Heatmap
-  Health Indicator Comparisons

##  Model Evaluation

The models are evaluated using multiple metrics rather than relying only on accuracy.

| Metric | Purpose |
|---|---|
| Accuracy | Measures overall prediction correctness |
| Precision | Measures correctness of positive predictions |
| Recall | Measures ability to identify positive cases |
| F1-Score | Balances precision and recall |
| ROC-AUC | Measures classification performance across thresholds |
| PR-AUC | Provides additional insight for imbalanced classification |

##  Model Performance Visualization

The project includes multiple visualizations for evaluating and comparing the models.

### Model Comparison

Models are compared using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- PR-AUC

### Confusion Matrix

Confusion matrices are generated to analyze:

- True Positives
- True Negatives
- False Positives
- False Negatives

### ROC Curve

ROC curves are used to compare model performance across different classification thresholds.

### Precision-Recall Curve

Precision-Recall curves provide additional insight into model performance, particularly when the target classes are imbalanced.

##  Model Interpretability

The project also analyzes why models make their predictions.

### Random Forest Feature Importance

Feature importance is extracted from the Random Forest model to identify influential healthcare indicators.

### Logistic Regression Coefficients

Logistic Regression coefficients are analyzed to understand the direction and relative influence of different features.

This makes the project more than a simple prediction system by providing insights into the underlying data.

##  Cross-Validation

Cross-validation is performed to evaluate the consistency and generalization of the Machine Learning models.

It helps determine whether the models:

- Generalize well
- Are sensitive to a particular train-test split
- Show signs of overfitting
- Produce stable results

##  Overfitting & Underfitting Analysis

The project compares training and testing performance to investigate model generalization.

### Overfitting

A model may be overfitting when:

Training Performance >> Testing Performance

This can indicate that the model has learned patterns specific to the training data.

### Underfitting

A model may be underfitting when:

Training Performance ≈ Testing Performance
AND
Both performances are relatively low

Learning curves and train-test comparisons are used to investigate these behaviors.

##  Error Analysis

The project includes dedicated error analysis to understand incorrect predictions.

The analysis focuses on:

- False Positives
- False Negatives
- Misclassified observations
- Prediction probabilities
- Class imbalance
- Model generalization

### False Negative Analysis

In a healthcare risk-prediction context, false negatives are important because they represent positive-class observations that the model fails to identify.

Therefore, Recall is analyzed alongside Precision, F1-Score, ROC-AUC, and PR-AUC.

##  Key Analytical Questions

The project investigates questions such as:

- Which health indicators are associated with diabetes risk?
- How does BMI differ across target classes?
- How does general health relate to diabetes risk?
- How do Logistic Regression, Decision Tree, and Random Forest compare?
- How stable are the models through cross-validation?
- Are there signs of overfitting or underfitting?
- What types of prediction errors occur?
- Which features contribute most to model predictions?

##  Technologies Used

### Programming

- Python

### Data Science & Visualization

- Pandas
- NumPy
- Matplotlib
- Seaborn

### Machine Learning

- Scikit-learn
- Logistic Regression
- Decision Tree
- Random Forest
- StandardScaler
- Cross-Validation
- Classification Metrics

### Concepts

- Data Cleaning
- Exploratory Data Analysis
- Data Preprocessing
- Classification
- Model Evaluation
- Feature Importance
- Error Analysis
- Model Interpretability
- Overfitting & Underfitting


##  How to Run

### 1. Clone the Repository

git clone https://github.com/rohanbhowm25308/Diabetes-Risk-Prediction-Healthcare-Analytics.git

### 2. Navigate to the Project

cd Diabetes-Risk-Prediction-Healthcare-Analytics

### 3. Install Dependencies

pip install pandas numpy matplotlib seaborn scikit-learn jupyter

### 4. Launch Jupyter Notebook

jupyter notebook

### 5. Open the Notebook

Diabetes_Risk_Prediction_and_Healthcare_Analytics.ipynb

### 6. Run All Cells

Execute the notebook cells sequentially to reproduce the complete analysis, visualizations, model training, and evaluation.

##  Project Outputs

The notebook produces:

- ✔ Data Cleaning
- ✔ Exploratory Data Analysis
- ✔ Target Distribution Analysis
- ✔ Healthcare Feature Analysis
- ✔ Correlation Heatmap
- ✔ Multiple ML Models
- ✔ Classification Metrics
- ✔ Confusion Matrices
- ✔ ROC Curves
- ✔ Precision-Recall Curves
- ✔ Feature Importance
- ✔ Logistic Regression Coefficients
- ✔ Cross-Validation Results
- ✔ Learning Curve
- ✔ Error Analysis
- ✔ Model Comparison
- ✔ Healthcare Analytics Insights

##  Project Strengths

- Uses a large real-world healthcare dataset
- Covers the complete Machine Learning workflow
- Compares multiple classification algorithms
- Uses multiple evaluation metrics
- Includes detailed visualizations
- Considers class imbalance
- Includes model interpretability
- Performs error analysis
- Investigates overfitting and underfitting
- Uses cross-validation
- Generates meaningful analytical insights

##  Limitations

- The dataset is based on survey-derived health indicators.
- The project is not a clinical diagnostic system.
- The target classes are imbalanced.
- Correlation does not imply causation.
- Model performance depends on dataset quality and representativeness.
- Additional clinical variables could potentially improve predictions.
- External validation would be required before any real-world deployment.


##  Internship Relevance

This project demonstrates practical implementation of:

Python
↓
Data Cleaning
↓
Exploratory Data Analysis
↓
Data Preprocessing
↓
Machine Learning
↓
Model Evaluation
↓
Data Visualization
↓
Error Analysis
↓
Model Interpretability
↓
Data Science Reporting

The project was developed as part of a Data Science with Python internship and demonstrates the application of Machine Learning techniques to a real-world healthcare analytics problem.

##  Dataset Reference

Diabetes Health Indicators Dataset

The dataset is based on the CDC's Behavioral Risk Factor Surveillance System (BRFSS) and is available through the UCI Machine Learning Repository.

## 👨‍💻 Author

**Rohan Bhowmik**

B.Tech Computer Science & Engineering

AI / Machine Learning | Data Science | Python | Web Development

## ⭐ Project Highlights

 Healthcare Analytics  
 Machine Learning Classification  
 Exploratory Data Analysis  
 Model Performance Evaluation  
 Feature Importance  
 Cross-Validation  
 Error Analysis  
 Overfitting & Underfitting Analysis  
 Data Visualization  
 Python + Scikit-learn

---

⭐ If you find this project useful, consider giving the repository a Star!
