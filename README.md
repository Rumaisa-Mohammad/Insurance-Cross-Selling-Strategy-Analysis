
# Insurance Cross-Selling Prediction & Customer Analytics

## 📌 Project Overview

This project focuses on analyzing customer insurance data and building a data-driven cross-selling strategy for an insurance company. The goal is to identify existing customers who are most likely to purchase additional insurance products, thereby increasing revenue, improving customer retention, and maximizing Customer Lifetime Value (CLV).

The project covers:

- Business understanding of cross-selling in insurance
- Data cleaning and preprocessing
- Missing value treatment using business-driven rules
- Exploratory Data Analysis (EDA)
- Customer conversion analysis
- Feature engineering
- Predictive modeling for cross-selling opportunities

---

## 🎯 Business Problem

Cross-selling is the practice of offering additional insurance products to existing customers. The primary objectives are:

1. Increase revenue from existing customers.
2. Strengthen customer relationships and improve retention.
3. Increase Customer Lifetime Value (CLV).
4. Reduce the likelihood of customers switching to competitors. :contentReference[oaicite:0]{index=0}

### Insurance Products Considered

- Motor Insurance
- Health Insurance
- Travel Insurance
- Personal Accident Insurance
- Householder Insurance
- Shopkeeper Insurance
- Fire Insurance
- Marine Insurance
- Industry Insurance
- Liability Insurance
- Micro Insurance
- Credit Insurance :contentReference[oaicite:1]{index=1}

## 🛠 Data Engineering Strategy

### Missing Value Treatment

| Variable             | Strategy                                                        |   |
| -------------------- | --------------------------------------------------------------- | - |
| Age                  | Replace missing values using the lower of Mean or Median        |   |
| Family Members       | Replace with Median                                             |   |
| Education            | Replace with Mode                                               |   |
| Occupation           | Replace with Mode                                               |   |
| Job Title            | Replace with Mode                                               |   |
| Income               | Occupation-wise Mean/Median based imputation                    |   |
| Current Product      | Business-rule based derivation                                  |   |
| Current Product Type | Conditional imputation using product information                |   |
| Current Coverage     | Product-type-based Mean/Median imputation                       |   |
| New Product Type     | Replace with Mode                                               |   |
| New Coverage         | Product-type-based Mean/Median imputation                       |   |
| Rating               | Product-type-wise Mode imputation                               |   |
| Converted            | Predictive imputation (e.g., KNN) instead of direct replacement |   |

---

## 🔄 Cross-Selling Scenarios

### Case 1: New Coverage > Current Coverage

Customers already insured under one product are offered additional insurance products, increasing their total coverage amount. 

### Case 2: New Coverage = Current Coverage

Customers whose existing policy has expired are offered a new product with equivalent coverage. 

### Case 3: New Coverage < Current Coverage

Customers whose existing policy has expired are offered a new insurance product with lower coverage. 

---

## 📊 Exploratory Data Analysis

The project performs:

### Univariate Analysis

* Conversion Status Distribution
* Income Distribution
* Customer Rating Analysis

### Bivariate Analysis

* Rating vs Conversion
* Income vs Conversion
* Customer Demographics vs Conversion

### Visualizations

* Histograms
* Count Plots
* Bar Charts
* Correlation Analysis
* Customer Conversion Insights

---

## 🤖 Machine Learning Workflow

1. Data Collection
2. Data Cleaning
3. Missing Value Treatment
4. Feature Engineering
5. Exploratory Data Analysis
6. Cross-Sell Prediction


## 📈 Business Benefits

* Improved customer loyalty
* Increased sales revenue
* Better customer retention
* Higher customer satisfaction
* Increased Customer Lifetime Value (CLV) 

---

## 🚀 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

## 📌 Conclusion

The project enables insurance companies to identify customers with a high probability of purchasing additional insurance products, helping maximize revenue while improving customer experience through targeted cross-selling campaigns.


