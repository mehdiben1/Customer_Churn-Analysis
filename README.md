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
 - Similar to Gender, the churn rate for customers with or without Phone Service is nearly identical (**26.75%** vs. **25%**). This suggests that Phone Service does not play a significant role in influencing churn behavior, making it a less critical factor for targeted retention strategies.
 - Customers with **fiber optic** internet service are significantly more likely to churn compared to those using other options. Specifically:

   - Fiber optic users churn at a rate of **49.89%**, which is **2.6 times** higher than customers with DSL (**19%**).
   - The churn rate for fiber optic users is even more pronounced when compared to customers with no internet service, who churn at a rate of just **7.43%**, making it approximately **6.7 times** higher.
 - The heat map below reveals that **customers using both fiber optic and phone services** experience the highest churn rate (**41.89%**). This subgroup may be facing issues related to bundled services, such as high costs. On the other hand, customers with DSL and phone services also exhibit a notable churn rate (**25%**), though it is less critical compared to fiber optic users. 
 
![Core Services](https://github.com/user-attachments/assets/df5efb2b-39f9-458b-ae0f-7fa6f1d476b7)

### b. Security Services:
-
-
-
-
![Security Services](https://github.com/user-attachments/assets/9d838ae8-4e0a-44c6-b811-b159cdab9262)

## 3. 
These findings suggest that customers who do not subscribe to security-related services (Online Security, Device Protection, Online Backup, or Tech Support) are at a higher risk of churn. 
   - Online Backup : For customers with an online backup service the churn rate is **21.57%**  and for those without this service the churn rate is **39.94%**
   - Device Protection: For Customers with a device Protection subscription the churn rate is **22.54%** in the other hand those who do not subscribe to this service the churn rate is **39.14%**
   - Online Security: For customers with an online security service the churn rate is **14.64%**  and for those without this service the churn rate is **41.78%**
   - Tech Support: Customers without Tech support churn at a rate of **41.65%**, which is **2.7 times** higher than Tech Support users (**15.20%**).
Tech Support and Online Security stand out as the most critical services, with the largest gap in churn rates. Customers without Tech Support may face unresolved technical issues, which may lead to dissatisfaction and eventual churn.
