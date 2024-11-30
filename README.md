# Project Background:
**Phonenow** is a medium-sized telecommunications company established in 2005. With approximately 15% of the national market share, the company serves over **1 million customers**, generating revenue from three main segments:
- **Internet Services (40%)**
- **mobile services (35%)**
- **TV services (25%)**
  
Recently, Phonenow has faced a significant challenge with customer churn, reaching a concerning rate of **26.54%**. This trend has resulted in  a substantial revenue loss of **$2.6 million**. With increasing competition in the telecommunications sector, retaining customers has become more critical than ever to sustain profitability and market share.
As a Data Analyst for Phonenow, my role was to identify the key characteristics of customers most likely to churn (at risk of leaving) by analyzing historical customer data. The analysis focused on uncovering **churn rate** patterns across three key dimensions:

- **Demographics:** age, Partner, dependents, Senior Citizen
- **Service usage:** phone services, Internet services
- **Contract & billing:** payment method, contract type, tenure ...

By uncovering these patterns, the analysis provides actionable insights to help Phonenow design targeted retention strategies, reduce churn rates, and improve customer loyalty.

# Data Structure:
The company main database structure as seen below consists of one table called **Customer_Chun**, with a total row count of **7033 records** and **21 columns**. Each record represents a single customer along with their associated information, including demographic details, the services they use, their contract and billing details and whether or not they have churned. Below is a brief description of the table contents:

![Capture d’écran 2024-11-30 154945](https://github.com/user-attachments/assets/5726948b-64fe-4919-86cf-2c28853df6de)

# Executive Summary:
## Overview of Findings


# Insights Deep Dive
## 1.  Churn rate Across Demographic variables:
- **Gender Does Not Significantly Affect Churn** : The churn rate is nearly identical between male and female customers(**26.96%** for female vs **26.20%** for male), indicating that gender is **not a distinguishing factor in churn behavior**.
- **Dependents Have a Strong Influence on Churn**:  Customers without dependents churn at **31.28%**, compared to **15.53%** for those with dependents,which could suggest that customers with dependents may prefer stability and long-term contracts."
- **For Partner Status, it Shows a Marginal Impact on Churn**, where the analysis showed that customers without partners churn at **32.98%**  compared to **19.72%** for those with partners. This aligns with patterns seen among customers without dependents, reinforcing the trend that single customers are at a higher risk of churning.
- **Senior Citizens Are at Greater Risk of Churning** where the churn rate among this category (**41.68%**) is significantly higher than that of younger customers (**23,65%**). This could be attributed to several factors, such as pricing sensitivity, preference for simpler plans, or service usability challenges.

 ![Demographic](https://github.com/user-attachments/assets/11070d6b-9434-4ed4-8d6f-0de8ecf74644)

 ## 2. Service usage:
 ### a. Core Services (Phone & Internet Services):
 -
 - Customer with fibre as internet service tend to churn more than those with Dsl
 
![Core Services](https://github.com/user-attachments/assets/df5efb2b-39f9-458b-ae0f-7fa6f1d476b7)

