## Customer Churn Prediction



## 📌 Problem Definition
The `Customer Churn table` contains information on all `7,043` customers from a `Telecommunications company` in California in Q2 2022

Each record represents `one customer`, and contains details about their `demographics`, `location`, `tenure`, `subscription services`, `status for the quarter` `(joined, stayed, or churned)`, and more!

The `Zip Code Population` table contains complimentary information on the estimated populations for the California zip codes in the Customer Churn table

We need to `predict` whether the customer will `churn`, `stay` or `join` the company based on the parameters of the dataset.
<br><br>

## 📓 Overview

| Machine Learning Models Applied            | Accuracy |
| ----------------- | ------------------------------------------------------------------ |
| Random Forest | 78.11% |
| Logistic Regression | 78.28% |
| Naive Bayes Gaussian | 36.77% |
| Decision Tree | 77.29% |
| XGB_Classifier | 80.86% |

<br>

## 👉 Application

The ability to predict churn before it happens allows businesses to take proactive actions to keep existing customers from churning. This could look like: 
```
  Customer success teams reaching out to those high-risk customers to provide support or to gauge 
  what needs may not be being met.
```

The advantage of calculating a company's churn rate is that it provides clarity on how well the business is retaining customers, which is a reflection on the quality of the service the business is providing, as well as its usefulness.

## 🔍 Data Exploration & Preprocessing

Before building the model, the data was carefully processed to ensure quality:

- **Handling Missing Data**: The `TotalCharges` column, which contained missing values, was cleaned or appropriately converted.
- **Data Type Conversion**: Some columns were cast from `object` to `float` to support further analysis.
- **Label Transformation**: Applied `Label Encoding` and `One-Hot Encoding` to handle categorical variables.
- **Data Balancing**: Checked label distribution and performed adjustments if necessary to improve model accuracy.

---

## 📊 Exploratory Data Analysis (EDA)

Initial data analysis provided valuable insights into customer behavior:

- Visualized the relationship between `churn` and other factors such as service types, payment methods, and tenure.
- Used bar charts, histograms, boxplots, and heatmaps to detect trends, outliers, and correlations in the data.

---

## ⚙️ Model Training & Evaluation

Several models were trained and their performances were compared:

- **Data Splitting**: 80% for training and 20% for testing.
- **Data Normalization**: Used `StandardScaler` to ensure consistent model performance.
- **Model Training**: Applied Logistic Regression, Random Forest, Decision Tree, Gaussian Naive Bayes, and XGBoost.
- **Model Evaluation**: Based on `Accuracy`, along with `Confusion Matrix`, `Precision`, `Recall`, and `F1-score`.

---

## 📈 Visualization

Data and results were visualized clearly:

- Confusion matrices for each model  
- Accuracy comparison across algorithms  
- Distribution plots of customers by churn status  
- ROC Curves for classification performance (if applicable)

---

## 💡 Insights

Key findings from the analysis:

- Postpaid customers using multiple services simultaneously are more likely to churn.
- The shorter the customer tenure, the higher the likelihood of churn.
- Some geographic regions showed significantly higher churn rates.

---

## 📬 Contact

For questions or contributions, please feel free to reach out:

- 📧 Email: [luudoanngocphat@gmail.com](mailto:luudoanngocphat@gmail.com)  
- 📞 Phone: 0905939655

