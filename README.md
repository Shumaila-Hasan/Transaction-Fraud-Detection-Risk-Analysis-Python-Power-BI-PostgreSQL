# Transaction-Fraud-Detection-Risk-Analysis-Python-Power-BI-PostgreSQL

#### Introduction

This project analyzes **1 million financial transactions across 50,000 accounts** to identify fraudulent transaction patterns, high-risk customer behavior, security vulnerabilities, and potential fraud networks.

The analysis combines transaction-level data with account profiles, fraud-pattern statistics, network relationships, and time-based transaction behavior. Using **Python, PostgreSQL, SQL, and Power BI**, the objective was to transform raw transaction data into actionable insights that can help a financial institution detect suspicious activity earlier, prioritize high-risk accounts, and reduce potential fraud losses.

### Problem Statement

Financial institutions process a large volume of transactions every day, making it difficult to identify fraudulent activity using transaction amount alone. Fraud can be associated with unusual transaction behavior, unknown devices, foreign transactions, high transaction velocity, weak authentication, suspicious accounts, and coordinated networks of accounts.

The business needs to understand **where fraud is occurring, which behaviors are strongly associated with fraud, which accounts and transaction patterns require immediate attention, and where fraud prevention controls can be strengthened**.

The project therefore focuses on identifying the major drivers of fraud and translating them into practical actions for **fraud detection, account monitoring, authentication controls, and loss reduction**.

### Goal

The goal of this project is to:

* Quantify the overall **fraud volume, fraud rate, and financial loss**.
* Identify transaction behaviors strongly associated with fraudulent activity.
* Detect **high-risk accounts and suspicious transactions**.
* Identify the most significant **fraud patterns and merchant categories**.
* Analyze temporal patterns to determine when fraud risk is highest.
* Identify suspicious relationships and potential **fraud rings**.
* Provide business recommendations that can help reduce fraud exposure and improve transaction monitoring.

### Tools & Technologies

-Python

Pandas
Data cleaning
Exploratory data analysis
KPI calculation

-SQL / PostgreSQL

Aggregations
CASE WHEN
CTEs
Window functions
Date/time analysis
Fraud segmentation

-Power BI

Interactive dashboard
KPI cards
Fraud trend analysis
Risk analysis
Merchant analysis
Transaction behavior analysis

### KPIs

KPI	                            Result
Total Transactions	            1,000,000
Total Transaction Value	         $183.74M
Fraudulent Transactions	         17,143
Fraud Rate	                     1.71%
Fraud Transaction Value          $12.52M
Fraud Loss Rate	               6.81%
Total Accounts	                  50,000
Fraudster Accounts	            13,336

### Insights

1. Fraud has a disproportionate financial impact

Fraud accounted for only 1.71% of transactions, but fraudulent transactions represented 6.81% of total transaction value.

This indicates that focusing only on fraud volume can underestimate the financial impact.

2. Unknown devices are a major fraud indicator
   
Device Status	Fraud Rate

Known Device	0.87%

Unknown Device	8.72%

Transactions from unknown devices showed approximately 10× higher fraud rates than transactions from known devices.

3. High transaction velocity is strongly associated with fraud
   
Velocity	Fraud Rate

Normal Velocity	0.22%

High Velocity	5.63%

High-velocity transactions showed a substantially higher fraud rate, making transaction frequency an important risk signal.

4. Foreign transactions have elevated fraud risk
   
Transaction Type	Fraud Rate

Domestic	1.01%

Foreign	3.40%

Foreign transactions showed more than 3× the fraud rate of domestic transactions.

5. Fraud is concentrated in specific merchant categories

The highest fraud-rate categories were:

Crypto — 5.34%
Money Transfer — 4.13%
Gambling — 3.57%
Travel — 2.61%
Electronics — 2.28%
6. Card-not-present fraud is the largest fraud pattern

Card-not-present fraud represented 34.89% of fraudulent transactions, followed by:

Account Takeover — 20.02%
Card Present Stolen — 18.20%
Friendly Fraud — 10.07%

The top three patterns accounted for approximately 73% of fraudulent transactions.

7. Fraud risk is highest during late-night hours

Fraud rates were highest between approximately 12 AM and 5 AM, with the highest hourly fraud rate occurring around 2 AM at 2.93%.


### Business Recommendations

Based on the analysis:

-Implement risk-based transaction scoring using multiple fraud signals.
-Apply additional authentication for transactions from unknown devices.
-Introduce velocity-based monitoring for unusually frequent transactions.
-Strengthen monitoring of high-risk merchant categories such as crypto and money transfer.
-Increase monitoring during late-night/high-risk hours.
-Prioritize high-value suspicious transactions because fraud has a disproportionate financial impact.
-Strengthen account-takeover detection using combinations of device, location, velocity, and transaction-value signals.


### Power BI Dashboard

![Dashboard](https://github.com/Shumaila-Hasan/Transaction-Fraud-Detection-Risk-Analysis-Python-Power-BI-PostgreSQL/blob/main/Transaction-Fraud-Detection-Risk-Analysis.png)

### Conclusion

The analysis shows that fraud is relatively infrequent in transaction volume but has a disproportionately large financial impact. The overall fraud rate is **1.71%**, while fraudulent transactions account for **6.81% of total transaction value**, highlighting the importance of focusing on potential financial loss rather than transaction count alone.

The strongest behavioral indicators identified were **unknown devices and high transaction velocity**, with fraud rates of **8.72% and 5.63% respectively**, compared with much lower rates for known devices and normal transaction velocity. Foreign transactions, disabled 2FA, unusual transaction hours, and high-risk merchant categories also showed elevated fraud rates.

Fraud is concentrated in a small number of major patterns, with **card-not-present, account takeover, and stolen-card fraud accounting for approximately 73% of fraudulent transactions**. The network analysis also indicates that fraudulent activity can occur through connected groups of accounts, suggesting that transaction-level monitoring alone may not be sufficient.

Overall, the analysis supports a **multi-layered fraud detection strategy** combining transaction behavior, account risk, authentication signals, merchant risk, temporal patterns, and network relationships. This approach can help financial institutions identify suspicious activity earlier, prioritize investigations, and reduce potential fraud losses.






