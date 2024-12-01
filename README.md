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
Our analysis of customer churn at Phonenow reveals three critical insights: 
- Customer Demographics: Senior citizens, along with customers who lack dependents or partners, exhibit significantly higher churn rates.
- Account and Billing Factors: Month-to-month contracts, paperless billing, and electronic check payments correlate with elevated churn rates. This suggests an opportunity to encourage long-term contracts through incentives (e.g., discounts or added benefits), improve customer satisfaction with digital billing experiences, and address potential issues associated with electronic check payments, such as ease of use or perceived convenience.
- Service Subscriptions: While phone services are widely used, add-ons like Streaming TV or Movies do not substantially impact churn rates. This underscores the importance of reassessing the value of bundled services in driving customer retention and ensuring they align with customer preferences.
![Presentation1](https://github.com/user-attachments/assets/eeca7c10-7900-4db1-b50a-a8f770a34978)


# Insights Deep Dive
## 1.  Churn rate Across Demographic variables:
- **Gender Does Not Significantly Affect Churn** : The churn rate is nearly identical between male and female customers(**26.96%** for female vs **26.20%** for male), indicating that gender is **not a distinguishing factor in churn behavior**.
- **Dependents Have a Strong Influence on Churn**:  Customers without dependents churn at **31.28%**, compared to **15.53%** for those with dependents,which could suggest that customers with dependents may prefer stability and long-term contracts."
- **For Partner Status, it Shows a Marginal Impact on Churn**, where the analysis showed that customers without partners churn at **32.98%**  compared to **19.72%** for those with partners. This aligns with patterns seen among customers without dependents, reinforcing the trend that single customers are at a higher risk of churning.
- **Senior Citizens Are at Greater Risk of Churning** where the churn rate among this category (**41.68%**) is significantly higher than that of younger customers (**23,65%**). This could be attributed to several factors, such as pricing sensitivity, preference for simpler plans, or service usability challenges.

 ![Demographic](https://github.com/user-attachments/assets/11070d6b-9434-4ed4-8d6f-0de8ecf74644)

 ## 2. Service usage:
 ### a. Core Services (Phone & Internet Services):
 - Similar to Gender, the churn rate for customers with or without Phone Service is nearly identical (**26.75% vs. 25%**). This suggests that Phone Service does not play a significant role in influencing churn behavior, making it a **less critical factor** for targeted retention strategies.
 - Customers with **fiber optic** internet service are significantly more likely to churn compared to those using other options. Specifically:
   -  Fiber optic customers churn at a rate of **49.89%**, which is **2.6 times higher** than DSL users (**19%**) and approximately **6.7 times higher** than customers with no internet service (**7.43%**).
     
 - The heat map below reveals that **customers using both fiber optic and phone services** experience the highest churn rate (**41.89%**). This subgroup may be facing issues related to bundled services, such as high costs. On the other hand, customers with DSL and phone services also exhibit a notable churn rate (**25%**), though it is less critical compared to fiber optic users. 
 
![Core Services](https://github.com/user-attachments/assets/df5efb2b-39f9-458b-ae0f-7fa6f1d476b7)

### b. Security Services:
Security-related services play a significant role in customer retention. Our analysis revealed that customers without these services are significantly more likely to churn, highlighting the importance of these offerings.

- Online Backup: Customers without an Online Backup service churn at **39.94%**, nearly double the rate of those with the service (**21.57%**).

- Device Protection: Customers without a Device Protection subscription churn at **39.14%**, compared to **22.54%** for those with the service.

- Online Security: The churn rate for customers without Online Security is **41.78%**, nearly **3 times higher** than the **14.64%** rate for customers with this service.

- Tech Support: Customers without Tech Support churn at **41.65%**, which is **2.7 times higher** than the **15.20%** churn rate for Tech Support users.

Tech Support and Online Security stand out as the most critical services, with the largest gap in churn rates. Customers without these services may face unresolved technical issues, leading to dissatisfaction and eventual churn.

![Security Services](https://github.com/user-attachments/assets/9d838ae8-4e0a-44c6-b811-b159cdab9262)

### c. Entertainment Services:
- The charts reveal that customers who subscribe to Streaming Movies or Streaming TV services have a churn rate that is similar to or slightly lower than those who do not subscribe:

   - Streaming TV: **30.11%** for subscribers vs. **33.54%** for non-subscribers.
   - Streaming Movies: **29.75%** for subscribers vs. **33.73%** for non-subscribers.
     
These findings indicate that streaming services (Movies or TV) **are not a significant factor in influencing customer churn behavior**.

![Entertainment Services](https://github.com/user-attachments/assets/4fe56a4c-5168-4416-974e-713b73c41cad)


## 3. Contract & Billing:
#### Contract 

- Customers with **shorter subscription times** (tenure ≤ 1 year) exhibit the highest churn rates (**47.68%**), indicating that customers with longer tenure are more loyal.
- Month-to-month contracts stand out with a churn rate of **42.71%**, which is nearly **4 times higher** than one-year contracts (**11.28%**) and **15 times higher** than two-year contracts (**2.85%**). This suggests that customers on month-to-month plans are less committed and more likely to leave.

#### Billing & Payment Preferences
- Customers paying via electronic checks have the highest churn rate (**45.29%**). This could be due to dissatisfaction or perceived inconvenience associated with this payment method.
- Customers opting for paperless billing have a churn rate of **33.59%**, which is **significantly higher** than those receiving physical bills (**16.38%**).
![Contract Billing](https://github.com/user-attachments/assets/69b32839-e9a0-45a6-a0b3-2d60eadcccc6)

# Recommendations:

