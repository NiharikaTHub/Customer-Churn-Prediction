# Customer-Churn-Prediction

## Introduction:

This project addresses the critical challenge of predicting customer churn within the banking sector. Customer departures from banking services have significant implications, affecting both revenue and operational efficiency. This project utilizes binary classification models to delve into the complexities of customer churn. The dataset includes diverse customer attributes such as credit score, country, gender, and more. Our primary objective is to provide insights that inform targeted retention strategies, ultimately enhancing customer satisfaction and loyalty in the dynamic banking industry.

<div align="center">
  <img src="https://github.com/NiharikaTHub/Customer-Churn-Prediction/assets/171478142/59ffb238-ada0-4da3-bcaa-fab30611cf1d" alt="Customer Churn Prediction" width="500"/>
</div>

## Tech Stack:

* Python (Programming Language)
* Pandas (Data Manipulation)
* Scikit-learn (Machine Learning Library)
* Matplotlib (Data Visualization)
* Seaborn (Statistical Data Visualization)

## Exploratory Data Analysis (EDA):

<div align="center">
  <img width="533" alt="Screenshot 2024-06-03 at 11 48 58 AM" src="https://github.com/NiharikaTHub/Customer-Churn-Prediction/assets/171478142/b0be05df-5e01-4620-ab9c-31980277bb58">
</div>

Through meticulous EDA, we gained a comprehensive understanding of the data:

* **Dataset Overview:** The dataset comprises 10,000 rows and 12 columns, representing various customer attributes. No duplicates or missing values were found. Key statistics include an average credit score of 650, a customer age range of 18 to 92 years, and an average tenure of 5 years.
* **Churn Distribution:** The bank's churn rate is 20.4%, indicating potential issues in customer satisfaction and loyalty.
* **Feature Distributions:** Violin plots and other visualizations revealed the distributions of key features such as credit score, age, tenure, balance, number of products, and estimated salary.
* **Credit Score by Churn and Gender:** Higher credit scores correlate with lower churn rates, regardless of gender.
* **Age Categories:** Adults (30-40 years) constitute the majority of the dataset.
* **Number of Products Purchased with Churn by Country:** Customers with two products are less likely to churn, with notable differences across countries.
* **Balance by Churn:** Retained customers often have low or zero balances, while churned customers show a more even distribution.

## Data and Methodology:

### Data Acquisition and Cleaning

  * **Data Collection:** The dataset includes customer attributes and churn status.
  * **Data Cleaning:** No duplicates or missing values were found.

### Feature Engineering

  * **New Features:** Introduced features such as age category, balance-salary ratio, credit score category, above-average balance, salary per product, and churn rate by country.
  * **Standardization:** Applied to ensure consistent scale across features, transforming each to have zero mean and unit variance.

## Model Selection and Evaluation:

* **Train-Test Split:**

Divided the data into training (80%) and testing (20%) sets.
  
* **Models Implemented:**

The analysis of models for predicting customer churn in the banking sector showed that Logistic Regression provided a solid baseline with 80.6% accuracy, while K-Nearest Neighbors (KNN) outperformed it with 83.9% accuracy, demonstrating KNN's superior ability to identify potential churners. Further exploration with Decision Tree and XGBoost models revealed that the Decision Tree had a lower accuracy of 78.15%, indicating its limitations in capturing complex data relationships, whereas XGBoost achieved the highest accuracy of 86.5%, showcasing its exceptional predictive capabilities through its advanced ensemble learning approach.

## Results:

| Model                     | Accuracy |
|---------------------------|----------|
| Logistic Regression       | 80.6%    |
| K-Nearest Neighbors (KNN) | 83.9%    |
| Decision Tree             | 78.15%   |
| **XGBoost**                   | **86.5%**    |


## Conclusion:

This study aimed to address the challenge of customer churn in banking by developing effective prediction models. The analysis revealed a high churn rate of 20.4%, highlighting potential issues in client satisfaction and loyalty. Our models provided actionable insights for implementing retention strategies. The K-Nearest Neighbors (KNN) and XGBoost models demonstrated robust predictive capabilities, with XGBoost achieving the highest accuracy at 86.5%. These findings underscore the importance of model selection in effectively addressing customer churn and enhancing customer satisfaction and loyalty.
