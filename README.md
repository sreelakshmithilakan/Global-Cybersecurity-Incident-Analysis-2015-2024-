# Global Cybersecurity Incident Analysis (2015–2024)
*Exploring Geographical, Industrial, Operational, and Temporal Risk Patterns in Global Cyber Attacks*

---

## 📌 Project Overview  
This project analyzes global cybersecurity incidents reported between **2015 and 2024** to identify **key risk patterns**, **attack trends**, and **defense effectiveness** across industries and countries.  
It demonstrates end-to-end **data cleaning**, **feature engineering**, **visual exploration**, and **insight reporting** using Python.

---

## 🎯 Objectives
- Understand **which countries and industries** are most impacted.
- Analyze the **most common attack types and exploited vulnerabilities**.
- Study relationships between **financial loss**, **user impact**, and **resolution time**.
- Identify **effective defense mechanisms** and **post-pandemic shifts** in cyber threat patterns.

---

## 🗂️ Dataset Description

| Column | Description |
|-------|-------------|
| Country | Location of the cybersecurity incident |
| Year | Year of occurrence |
| Attack Type | e.g., Malware, DDoS, Ransomware, Phishing |
| Target Industry | e.g., Finance, Healthcare, IT, Retail |
| Financial Loss (Million $) | Estimated monetary impact |
| Number of Affected Users | Total affected users |
| Attack Source | Internal or External actor |
| Security Vulnerability Type | Weak passwords, unpatched software, etc. |
| Defense Mechanism Used | Mitigation strategy |
| Incident Resolution Time (Hours) | Time required to resolve |

### 🔧 Derived Fields
- **Era** → (Pre-Pandemic, Pandemic, Recovery, Recent)
- **Resolution Bucket** → (≤24h, 24–72h, >72h)
- **Loss per User** → Financial Loss ÷ Users Affected

---

## 🧹 Data Preparation & Cleaning
- Standardized categorical labels
- Handled missing values and duplicates
- Converted datatypes appropriately
- Detected and adjusted outliers
- Engineered new analytical variables (Era, Resolution Bucket, Loss per User)

---

## 📊 Analysis Approach

### 1. **Univariate Analysis**
Understanding distributions:
- Top affected countries
- Most targeted industries
- Most common attack types

### 2. **Bivariate Analysis**
Comparing variables:
- Loss by country & industry
- Attack type vs vulnerability exploited
- Defense mechanism effectiveness vs resolution time

### 3. **Multivariate & Trend Analysis**
- Evolution of attacks from 2015–2024
- Pre- vs Post-Pandemic shifts
- Heatmaps & grouped plots across sectors

---

## 🔍 Key Insights

| Insight Area | Summary |
|-------------|---------|
| **High-Risk Regions** | UK, Brazil, Japan, and France show consistently high incident rates. |
| **Most Targeted Industries** | IT, Banking, and Healthcare face highest risk due to data sensitivity & value. |
| **Dominant Attack Types** | Phishing, Ransomware, and DDoS attacks are most common globally. |
| **Vulnerability Drivers** | Human error and unpatched software remain major root causes. |
| **Defense Effectiveness** | **AI-based threat detection** resolves incidents faster than traditional tools. |
| **Post-Pandemic Trends** | Spike in ransomware and SQL injection attacks during remote-work transition. |

---

## 🛠️ Tech Stack
| Tool | Purpose |
|------|---------|
| **Python (Pandas, NumPy)** | Data Cleaning & Feature Engineering |
| **Matplotlib / Plotly** | Data Visualization |
| **Jupyter Notebook** | Analysis & Documentation |

---

