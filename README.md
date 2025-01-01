# 🧾 PowerCo Customer Churn Analysis

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)[![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)](#)  [![Platform](https://img.shields.io/badge/Platform-Jupyter-orange.svg)](#)

---

## 📌 Project Overview

PowerCo, a prominent utility provider, is navigating challenges in the competitive energy market, where **customer churn** poses a critical threat to revenue and market share. This project investigates the drivers of churn, with a particular focus on **price sensitivity** and other contributing factors like customer behavior, demographics, and contract details.  

By leveraging advanced data analytics and machine learning, the goal is to identify actionable strategies to enhance customer retention and maintain PowerCo's competitive edge.

---

## 🎯 Objectives

- **Evaluate the Impact of Price Sensitivity**: Assess if price sensitivity, particularly changes in off-peak pricing, is a significant predictor of churn.
- **Analyze Alternative Factors**: Examine how customer consumption patterns, demographics, and contract details contribute to churn.
- **Develop Predictive Models**: Build machine learning models to uncover the key drivers of churn.
- **Provide Actionable Insights**: Recommend strategies to reduce churn and improve customer retention.

---


## 📊 Methodology

### 1. **Exploratory Data Analysis (EDA)**
- **Dataset**: Includes customer data on pricing, consumption, contract details, and churn.\n
- **Steps**:
  - Checked for missing and duplicate values, ensuring data integrity.
  - Analyzed distributions, outliers, and variable correlations.
  - Visualized key trends using box plots, histograms, and heatmaps.
- **Key Observations**:
  - Significant class imbalance: 90.28% non-churned vs. 9.72% churned customers.
  - Consumption patterns exhibited strong correlation with churn.
  - Price variables alone showed weak correlation with churn.

### 2. **Hypothesis Testing**
- **Null Hypothesis (H0)**: No significant relationship between price sensitivity and churn.
- **Findings**:
  - Price sensitivity alone is not a strong predictor of churn (p-values > 0.05).
  - Other factors, such as customer engagement and satisfaction, likely play a more critical role.

### 3. **Feature Engineering**
- Created meaningful features to improve model accuracy:\n
  - **Price Difference Metrics**: Captured changes in pricing across periods.\n
  - **Consumption Deviations**: Measured unusual consumption patterns.\n
  - **Customer Tenure**: Derived loyalty insights.\n
  - **Categorical Encoding**: Converted non-numerical variables for compatibility with machine learning models.

### 4. **Model Development**
- Implemented and evaluated multiple models:\n
  - **Random Forest**: Achieved the best performance with 99% accuracy and balanced precision/recall.\n
  - **Logistic Regression**: Struggled with imbalanced data (poor recall for churned customers).\n
  - **XGBoost**: Performed well for non-churned customers but underperformed for churn detection.


---


## 📋 Key Findings

- **Price Sensitivity**: Changes in pricing have limited influence on churn.\n
- **Consumption Patterns**: Deviations in usage trends are the strongest indicators of churn.
- **Tenure and Cohorts**: Early onboarding strategies are crucial, as newer customers exhibit higher churn rates.
- **Class Imbalance**: Addressing imbalanced datasets is critical for improving model performance.

**Refer Document**: 📄 **[PowerCo Analysis Report.pdf](https://github.com/user-attachments/files/18284824/PowerCo.Analysis.Report.pdf)**


---


## 📂 Repository Contents

### **1. Reports**
- 📄 **[PowerCo Analysis Report.pdf](https://github.com/user-attachments/files/18284824/PowerCo.Analysis.Report.pdf)**: Detailed analysis and recommendations.

### **2. Code & Notebooks**
- 📂 **`notebooks/`**: Jupyter notebooks for analysis and modeling.\n
  - `data_exploration.ipynb`: Comprehensive EDA.\n
  - `feature_engineering.ipynb`: Advanced feature creation.\n
  - `model_building.ipynb`: Model training, evaluation, and hyperparameter tuning.

### **3. Resources**
- 📂 **`data/`**: Includes raw and processed datasets (restricted for privacy).\n
- 📂 **`visualizations/`**: Charts and graphs from the analysis.

### **4. Documentation**
- 📄 **`README.md`**: Project description and guide.\n
- 📄 **`LICENSE`**: Licensing details.


---

## 🚀 Getting Started

### **1. Clone the Repository**
```bash
git clone https://github.com/your-username/your-repository.git
cd your-repository
```
### **2. Install Dependencies**
```bash
pip install -r requirements.txt
```
### **3. Run the Notebook**
```bash
jupyter notebook
```

---

## 🛠️ Technologies and Tools

- Python 3.8+
- **Libraries**: **`pandas`**, **`numpy`**, **`scikit-learn`**, **`xgboost`**, **`matplotlib`**, **`seaborn`**
- **Tools**: Jupyter Notebook, GitHub, Visual Studio Code

---

## ✨ Recommendations
- **Monitor High-Risk Customers**: Use consumption patterns to proactively identify and engage at-risk clients.
- **Enhance Onboarding**: Focus on customer engagement during the first two years of tenure.
- **Optimize Pricing Strategies**: Introduce selective discounts targeting high-risk segments.
- **Model Enhancements**: Address class imbalance using SMOTE or cost-sensitive learning.

---

## 🏆 Contributions

Contributions, issues, and feature requests are welcome! Feel free to fork the repository and make improvements.

---

## 📧 Contact

- **Author**: Mohammad Adnan
- **Email**: adnan.bava123@gmail.com
