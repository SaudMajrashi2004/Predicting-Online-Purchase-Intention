# 🛒 Predicting Online Purchase Intention

## 📌 Project Overview

This project focuses on predicting whether an online shopping session will result in a purchase based on visitors' browsing behavior.

The project combines **Data Analysis, Business Analytics, and Machine Learning** to transform online browsing-session data into useful business insights and predictive results.

---

## ❓ Business Problem

Online businesses receive a large number of website sessions, but only a small percentage of these sessions result in a purchase.

This raises an important business question:

> **How can an online business identify website visitors who are more likely to make a purchase based on their browsing behavior?**

Understanding these patterns can help businesses improve customer targeting, website experience, and conversion strategies.

---

## 💡 Project Solution

This project addresses the problem by analyzing **12,330 online shopping sessions** and building machine learning models to predict whether a browsing session will result in a purchase.

The project follows an end-to-end workflow:

**Business Understanding → Data Collection → Data Understanding → Data Cleaning → EDA → Data Preprocessing → Model Building → Model Evaluation → Business Insights**

---

## 📂 Dataset

The dataset used is the **Online Shoppers Purchasing Intention Dataset**.

- **Rows:** 12,330
- **Input Features:** 17
- **Target Variable:** `Revenue`
- `Revenue = True` → Purchase
- `Revenue = False` → No Purchase

The dataset contains information about visitors' browsing behavior, including:

- Product-related pages
- Administrative pages
- Informational pages
- Time spent on different page types
- Bounce Rate
- Exit Rate
- Page Values
- Visitor Type
- Traffic Type
- Weekend
- Month

---

# 📊 Exploratory Data Analysis

Several visualizations were created to understand visitor behavior and identify patterns related to purchasing.

## 📸 Key Visualizations

The following visualizations were selected to highlight the **key stages and findings of the project**, from understanding the data and exploring customer behavior to evaluating the machine learning models and identifying the most important features.

Other visualizations are available in the project notebook.

---

### 1. 📊 Revenue Distribution

This visualization shows the distribution of sessions between purchases and non-purchases.

The majority of sessions did not result in a purchase, while a smaller proportion resulted in a purchase. This highlights the **class imbalance** in the target variable.

![Revenue Distribution](images/revenue_distribution.png)

---

### 2. 👥 Purchase Rate by Visitor Type

This visualization compares purchase rates across different visitor types.

It helps identify differences in purchasing behavior between visitor segments and can support customer segmentation strategies.

![Purchase Rate by Visitor Type](images/purchase_rate_visitor_type.png)

---

### 3. 💰 PageValues vs Revenue

This analysis examines the relationship between `PageValues` and purchase behavior.

`PageValues` was also identified as the **most important feature** in the Random Forest model, making it an important predictive signal in this dataset.

![PageValues vs Revenue](images/page_value_vs_revenue.png)

---

### 4. 🛍️ Product-Related Browsing Behavior

This visualization compares time spent on product-related pages between purchasing and non-purchasing sessions.

It provides insight into how product-page engagement is associated with purchase behavior.

![Product Related Browsing Behavior](images/product_related_duration_vs_revenue.png)

---

### 5. 🔗 Correlation Matrix

The correlation matrix shows relationships between numerical variables in the dataset.

It helps understand the structure of the data and identify relationships between behavioral features before building the machine learning models.

![Correlation Matrix](images/correlation_matrix.png)

---

# 🤖 Machine Learning

Two classification models were developed and compared.

## 1. Logistic Regression

Logistic Regression was used as a baseline classification model.

### Results

- **Accuracy:** 88.94%
- **Precision:** 77.18%
- **Recall:** 41.62%
- **F1-Score:** 54.08%

---

## 2. Random Forest

Random Forest was developed to capture more complex relationships between the behavioral features.

### Results

- **Accuracy:** 90.82%
- **Precision:** 76.87%
- **Recall:** 59.16%
- **F1-Score:** 66.86%

---

## 🎯 Random Forest Confusion Matrix

The confusion matrix shows how the Random Forest model classified purchasing and non-purchasing sessions.

The model correctly identified **226 purchasing sessions**, while **156 actual purchasing sessions were incorrectly classified as non-purchases**.

![Random Forest Confusion Matrix](images/random_forest_confusion_matrix.png)

---

# ⭐ Feature Importance

Random Forest feature importance was used to identify the features that contributed most to the model's predictions.

`PageValues` was the most influential feature, followed by product-related browsing behavior and other behavioral indicators such as `ExitRates` and `BounceRates`.

> Feature importance indicates predictive usefulness within the model and should not be interpreted as causal impact.

![Feature Importance](images/feature_importance.png)

---

# 📈 Model Performance Comparison

The two models were evaluated using four classification metrics:

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| Logistic Regression | 88.94% | 77.18% | 41.62% | 54.08% |
| Random Forest | 90.82% | 76.87% | 59.16% | 66.86% |

Random Forest achieved higher **Accuracy, Recall, and F1-Score**, while Logistic Regression had slightly higher **Precision**.

![Model Performance Comparison](images/model_comparison.png)

---

# 💼 Key Business Insights

Based on the analysis and model results:

- `PageValues` was the most influential predictive feature.
- Product-related browsing behavior showed an important relationship with purchase behavior.
- `ExitRates` and `BounceRates` provided useful behavioral signals.
- Purchase behavior varied across visitor types.
- Traffic sources and seasonal patterns can provide additional information about purchasing behavior.
- The target variable is imbalanced, with non-purchasing sessions representing the majority of observations.

---

# 💡 Business Recommendations

Based on the findings, businesses could:

1. **Improve product pages** to encourage visitors to continue through the purchasing journey.
2. Analyze pages with high **Exit Rates and Bounce Rates** to identify potential usability problems.
3. Use browsing behavior to identify **high-potential sessions**.
4. Develop different strategies for **new and returning visitors**.
5. Analyze traffic sources based on **conversion quality**, not only traffic volume.
6. Consider seasonal purchasing patterns when planning marketing campaigns.
7. Use **A/B testing** to validate whether website or marketing changes improve conversion rates.

---

# 🛠️ Technologies & Tools

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Google Colab
- Jupyter Notebook
- GitHub

---


# 🏁 Conclusion

This project demonstrates an end-to-end machine learning workflow for predicting online purchase intention.

After performing data analysis, preprocessing, model development, and evaluation, **Random Forest achieved 90.82% accuracy and a 66.86% F1-score**.

The project also demonstrates how machine learning can be combined with **business analysis and data analytics** to identify behavioral patterns and generate actionable business insights.

---

## 👨‍💻 Skills Demonstrated

**Data Analysis | Exploratory Data Analysis | Data Preprocessing | Machine Learning | Classification | Model Evaluation | Feature Importance | Business Insights | Business Recommendations**

---

# 👨‍💻 About Me

**Saud Majrashi**

Management Information Systems (MIS) Student

Interested in:

- Data Analytics
- Business Intelligence
- Business Analysis
- Machine Learning

This project reflects my interest in combining **business understanding, data analysis, and technology** to solve real-world business problems.

### 🔗 Connect With Me

- GitHub: [SaudMajrashi2004](https://github.com/SaudMajrashi2004)
- LinkedIn: [LinkedIn Profile](YOUR_LINKEDIN_URL)

---

⭐ If you found this project useful, feel free to explore the repository and the notebook.
