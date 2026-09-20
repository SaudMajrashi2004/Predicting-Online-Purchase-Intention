# 🛒 Predicting Online Purchase Intention

## 📌 Project Overview

This project predicts whether an online shopping session will result in a purchase based on visitors' browsing behavior.

It combines **Data Analytics, Business Analytics, and Machine Learning** to transform website-session data into predictive insights that can support customer targeting, conversion optimization, and business decision-making.

---

## 👨‍💻 What I Did

In this project, I completed the end-to-end analytical workflow, including:

- Data understanding and validation
- Data cleaning and preparation
- Exploratory Data Analysis (EDA)
- Data preprocessing
- Feature preparation
- Machine learning model development
- Model evaluation and comparison
- Feature importance analysis
- Business insight generation
- Business recommendations

---

## 🔎 Quick Access

- [View Project Notebook](online_purchase_intention_prediction.ipynb)
- [View Dataset](online_shoppers_intention.csv)

---

## ❓ Business Problem

Online businesses receive a large number of website visits, but only a relatively small proportion of sessions result in a purchase.

This raises an important business question:

> **How can an online business identify website visitors who are more likely to make a purchase based on their browsing behavior?**

Identifying these patterns can help businesses improve customer targeting, website experience, marketing effectiveness, and conversion strategies.

---

## 💡 Project Solution

This project analyzes **12,330 online shopping sessions** and develops machine learning models to predict whether a session will result in a purchase.

The project follows an end-to-end workflow:

**Business Understanding → Data Collection → Data Understanding → Data Cleaning → EDA → Data Preprocessing → Model Building → Model Evaluation → Business Insights**

---

## 📂 Dataset

The project uses the **Online Shoppers Purchasing Intention Dataset**.

- **Rows:** 12,330
- **Input Features:** 17
- **Target Variable:** `Revenue`
- `Revenue = True` → Purchase
- `Revenue = False` → No Purchase

The dataset includes information related to visitor behavior such as:

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

Exploratory Data Analysis was performed to understand visitor behavior, identify patterns related to purchasing, examine class distribution, and investigate relationships between important variables.

---

### 1. 📊 Revenue Distribution

The target variable shows an imbalance between purchasing and non-purchasing sessions.

Most website sessions did not result in a purchase, while a smaller proportion resulted in a successful transaction.

![Revenue Distribution](images/1-Revenue%20Distribution.png)

---

### 2. 👥 Purchase Rate by Visitor Type

Purchase behavior differs across visitor segments.

This analysis helps identify how visitor type is associated with conversion behavior and can support more targeted customer strategies.

![Purchase Rate by Visitor Type](images/2-Purchase%20Rate%20by%20Visitor%20Type.png)

---

### 3. 💰 PageValues vs Revenue

`PageValues` shows a strong relationship with purchase behavior.

The variable was also identified as the most influential feature in the Random Forest model, making it an important predictive signal in this dataset.

![PageValues vs Revenue](images/3-PageValues%20vs%20Revenue.png)

---

### 4. 🛍️ Product-Related Browsing Behavior

This analysis compares product-related browsing duration between purchasing and non-purchasing sessions.

It provides insight into how engagement with product pages is associated with purchase intention.

![Product Related Browsing Behavior](images/4-ProductRelated%20Duration%20vs%20Revenue.png)

---

### 5. 🔗 Correlation Matrix

The correlation matrix was used to examine relationships between numerical variables.

This helped understand the structure of the dataset and identify relationships between behavioral variables before model development.

![Correlation Matrix](images/5-Correlation%20Matrix.png)

---

# 🤖 Machine Learning

Two classification models were developed and evaluated:

- Logistic Regression
- Random Forest

The models were compared using:

- Accuracy
- Precision
- Recall
- F1-Score

---

## 1. Logistic Regression

Logistic Regression was used as the baseline classification model.

### Results

- **Accuracy:** 88.94%
- **Precision:** 77.18%
- **Recall:** 41.62%
- **F1-Score:** 54.08%

The model achieved relatively high precision but lower recall, meaning it was more conservative when identifying purchasing sessions.

---

## 2. Random Forest

Random Forest was used to capture more complex relationships between browsing behavior and purchase intention.

### Results

- **Accuracy:** 90.82%
- **Precision:** 76.87%
- **Recall:** 59.16%
- **F1-Score:** 66.86%

Compared with Logistic Regression, Random Forest improved the identification of actual purchasing sessions while maintaining strong overall predictive performance.

---

## 🎯 Random Forest Confusion Matrix

The confusion matrix provides a detailed view of the Random Forest classification results.

The model correctly identified **226 purchasing sessions**, while **156 actual purchasing sessions were classified as non-purchases**.

![Random Forest Confusion Matrix](images/6-Random%20Forest%20Confusion%20Matrix.png)

---

# ⭐ Feature Importance

Random Forest feature importance was used to identify the variables that contributed most to the model's predictions.

`PageValues` was the most influential predictive feature.

Other important behavioral variables included product-related activity, `ExitRates`, and `BounceRates`.

> Feature importance represents predictive usefulness within the model and should not be interpreted as causal impact.

![Random Forest Feature Importance](images/7-Random%20Forest%20Feature%20Importance.png)

---

# 📈 Model Performance Comparison

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| Logistic Regression | 88.94% | 77.18% | 41.62% | 54.08% |
| Random Forest | 90.82% | 76.87% | 59.16% | 66.86% |

Random Forest achieved higher **Accuracy, Recall, and F1-Score**, while Logistic Regression achieved slightly higher **Precision**.

![Model Performance Comparison](images/8-Model%20Performance%20Comparison.png)

---

# 💼 Key Business Insights

The analysis produced several useful business insights:

- `PageValues` was the strongest predictive feature in the Random Forest model.
- Product-related browsing behavior was associated with purchase intention.
- `ExitRates` and `BounceRates` provided useful signals about visitor behavior.
- Purchase behavior differed across visitor types.
- Traffic sources may provide useful information about conversion quality.
- Seasonal patterns may influence purchasing behavior.
- The target variable is imbalanced, with non-purchasing sessions representing the majority of observations.

---

# 💡 Business Recommendations

Based on the analysis, online businesses could consider the following actions:

1. **Improve product pages** to encourage visitors to continue through the purchasing journey.
2. Analyze pages with high **Exit Rates** and **Bounce Rates** to identify potential usability issues.
3. Use browsing behavior to identify **high-potential customer sessions**.
4. Develop different strategies for **new and returning visitors**.
5. Evaluate traffic sources based on **conversion quality**, not only traffic volume.
6. Consider seasonal purchasing patterns when planning marketing campaigns.
7. Use **A/B testing** to measure whether website changes actually improve conversion rates.

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

# 🧠 Skills Demonstrated

This project demonstrates practical experience in:

**Data Analysis | Exploratory Data Analysis | Data Cleaning | Data Preprocessing | Machine Learning | Classification | Model Evaluation | Feature Importance | Business Analytics | Business Insights | Business Recommendations**

---

# 🏁 Conclusion

This project demonstrates an end-to-end machine learning and business analytics workflow for predicting online purchase intention.

After completing data analysis, preprocessing, model development, and evaluation, the **Random Forest model achieved 90.82% accuracy and a 66.86% F1-score**.

The project also demonstrates how analytical and machine learning techniques can be connected to business problems to identify behavioral patterns and generate actionable insights.

---

# 👨‍💻 About Me

**Saud Majrashi**

Management Information Systems (MIS) Student

Interested in:

- Data Analytics
- Business Intelligence
- Business Analysis
- Machine Learning



### 🔗 Connect With Me

- GitHub: [SaudMajrashi2004](https://github.com/SaudMajrashi2004)
- LinkedIn: [LinkedIn Profile](www.linkedin.com/in/saud-majrashi)
