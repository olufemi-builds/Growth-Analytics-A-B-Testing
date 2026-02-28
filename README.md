
# 📈 Growth Analytics & A/B Testing

[![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)](https://python.org)
[![Pandas](https://img.shields.io/badge/Pandas-1.6-orange?logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![Statsmodels](https://img.shields.io/badge/Statsmodels-0.19-green?logo=python&logoColor=white)](https://www.statsmodels.org/)

---

## ## 📌 Project Overview
# 🌱 Growth Analytics Portfolio

**Technologies:** Python (Pandas, Statsmodels, NumPy), SQL, Power BI, Excel  

This portfolio demonstrates my ability to translate **complex business problems** into **data-driven insights**. Projects simulate real-world scenarios in **SaaS, e-commerce, fintech, and Big Tech**, emphasizing **A/B testing, growth analytics, product experimentation, and KPI frameworks**.

---

# **1. Growth Analytics & A/B Testing**

**Business Problem:**  
Product teams need to validate whether new features increase **conversion rates** and **revenue per user**. Poor decision-making without evidence can result in lost revenue and misaligned product strategies.

**Solution:**  
Performed **A/B testing analysis** using Python to measure conversion lift, revenue impact, and statistical significance. Built **data pipelines** and optional dashboards for decision-making.

**Step-by-Step Analysis (Python)**

```python
# Load libraries
import pandas as pd
from statsmodels.stats.proportion import proportions_ztest

# Load dataset
df = pd.read_csv("AB_Test.csv")
df.head()

# 1️⃣ Sanity Checks
df.info()
print("Conversion rates by group:\n", df.groupby("group")["converted"].mean())

# 2️⃣ Conversion Rate Analysis
conversion = df.groupby("group")["converted"].mean() * 100
print(f"\nConversion Rates (%):\n{conversion}")

# 3️⃣ Revenue Analysis
revenue = df.groupby("group")["revenue"].mean()
print(f"\nAverage Revenue per User:\n{revenue}")

# 4️⃣ Statistical Significance Test
control = df[df["group"]=="Control"]["converted"]
variant = df[df["group"]=="Variant"]["converted"]

count = [variant.sum(), control.sum()]
nobs = [len(variant), len(control)]

stat, pval = proportions_ztest(count, nobs)
print(f"\nP-Value: {pval}")

**Project Link:**  
[KPI & Dashboard Automation](https://github.com/olufemiolamoyegun/KPI-Dashboard-Automation)

---

# **Portfolio Highlights**
This portfolio showcases my ability to:  
- Translate business questions into **decision-ready analytics solutions**  
- Build **scalable dashboards** and **ETL pipelines**  
- Perform **statistical analysis and hypothesis testing**  
- Communicate insights effectively to **stakeholders and executives**  

---

# **Certifications**
- **PL-300:** Microsoft Power BI Data Analyst  
- **DP-600:** Microsoft Fabric Analytics Engineer  
- **Oracle Cloud AI Foundations**  
- **AWS Storage Knowledge Badge**  
- **Cisco Python Essentials 1 & 2**  
- **Business Intelligence & Data Analytics (BIDA™)**  

---

# **Portfolio Focus Areas**
- Business Intelligence & Operational Analytics  
- Product & Growth Analytics  
- Workforce & Organizational Analytics  

---

# **Author**
**Olufemi Olamoyegun**  
Senior Data Analyst | Power BI | SQL | Python | Microsoft Fabric  
🔗 [LinkedIn](https://www.linkedin.com/in/olufemiolamoyegun/) | 📂 [GitHub](https://github.com/olufemiolamoyegun)  

---

# **Portfolio Philosophy**
Data should not just **produce reports**—it should **drive business strategy, guide decisions, and create measurable impact**. This portfolio emphasizes:  
- Business problem framing  
- Analytical rigor  
- Actionable insights  
- Scalable analytics workflows

🔗 [LinkedIn](https://www.linkedin.com/in/olufemi-olamoyegun) | 📂 [GitHub](https://github.com/olufemiolamoyegun)









