# Global Cybersecurity Incident Analysis (2015–2024)
*Exploring Geographical, Industrial, Operational, and Temporal Risk Patterns in Global Cyber Attacks*

---

## 📌 Project Overview  
This project analyzes global cybersecurity incidents reported between **2015 and 2024** to identify **key risk patterns**, **attack trends**, and **defense effectiveness** across industries and countries.  
It demonstrates end-to-end **data cleaning**, **feature engineering**, **visual exploration**, and **insight reporting** using Python.

---

### 📁 Project Files

**data/**
- `Global_Cybersecurity_Threats.csv` — *Dataset used for analysis*

**notebooks/**
- `Global-Cybersecurity-Incident-Analysis.ipynb` — *Main Jupyter Notebook*

**images/**
- `Cybersecurity-project-images/` — *All visualizations generated during the analysis*

**README.md**
- *Project documentation you are currently reading*

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

### 4. **📈 Statistical Validation**

To strengthen insights obtained during exploratory analysis, statistical tests were applied to evaluate whether observed relationships are statistically significant.

| Relationship Tested | Method Used | Purpose |
|--------------------|-------------|--------|
| Year × Incident Count | Linear Regression | Evaluate whether cyber incidents show a statistically significant trend over time |
| Attack Type × Financial Loss | ANOVA | Test whether financial losses differ significantly across attack types |
| Affected Users × Financial Loss | Pearson Correlation | Examine whether incidents affecting more users tend to generate larger financial losses |

These statistical tests complement the visual analysis and help distinguish observable patterns from statistically meaningful relationships.

---

## 🔍 Key Insights (Table Summary)

| Insight Area | Summary |
|-------------|-----------------|
| **High-Risk Regions** | UK, Brazil, Japan, and Australia show **concentrated high-impact attack clusters**, while India and France show **moderate but steady exposure**. |
| **Most Targeted Industries** | **IT, Banking, Healthcare, and Education** face highest risk due to **centralized identity/financial data and operational dependence**. |
| **Dominant Attack Types** | **SQL Injection & Phishing** remain consistently prevalent; **Ransomware** increases significantly post-pandemic. **DDoS** remains stable but lower in share. |
| **Primary Vulnerabilities** | **Unpatched software + human behavior** (phishing/social engineering) remain the most exploited weaknesses. |
| **Defense Performance** | **Firewalls & Encryption** provide stable protection; **VPN and early AI-based systems struggled** during remote-work expansion. |
| **Pandemic Shift** | **Incident frequency decreased**, but **impact severity increased**, due to rapid digital expansion and limited adaptation time. |

---

## Detailed Insights

## 🌍 **Global Threat Landscape**

Cybersecurity risk is **global**, not concentrated in specific regions.  
Countries like **UK, Brazil, Japan, and Australia** report **higher visible incident volumes** due to **greater digital activity and transparent reporting**.  
Meanwhile, **USA, Germany, and China** show **lower reported incidents** due to **centralized monitoring and restricted disclosure**.

**Key Insight:**  
Higher incident counts can reflect **digital scale and transparency**, not weaker defense.

---

## 🎯 **Attack Type Patterns**

- **SQL Injection** and **Phishing** maintain consistent prevalence.
- **Ransomware** shows a **major increase post-2020**, tied to remote operational pressure.
- **DDoS** remains present but **stable at a lower share**.

**Key Insight:**  
Organizations need **multi-layered security**, not single-vector protection.

---

## 🏦 **Industry Exposure**

Industries with **high-value or identity-linked data** face the greatest risk:

- **IT & Banking** → high-value centralized data  
- **Healthcare** → **zero downtime tolerance** increases ransomware leverage  
- **Education** → large user bases, distributed access, often **lower cybersecurity budgets**

**Key Insight:**  
Attackers focus on sectors where **data sensitivity and continuity** matter most.

---

## 🧬 **User Exposure Patterns**

User exposure is highest in **IT, Healthcare, Education, and Banking**, where data is:

- **Centralized**
- **Identity-linked**
- **Widely accessed**

**Key Insight:**  
Impact increases when data is **centralized and personally identifiable**.

---

## 🔗 **Vulnerabilities and Exploitation**

- **Phishing** → exploits **human trust + zero-day openings**
- **Weak Passwords** → enable **botnet-driven DDoS**
- **Unpatched Software** → drives **Ransomware & MITM attacks**

**Key Insight:**  
Most breaches result from **human factors and delayed updates**, not attacker sophistication.

---

## 🛡️ **Defense Mechanism Effectiveness**

| Defense Approach | Reliability Trend | Notes |
|-----------------|------------------|------|
| **Firewalls & Encryption** | **Stable & effective** | Strong perimeter and data protection |
| **VPN & Early AI Detection** | **High loss during pandemic** | Struggled under sudden remote expansion |
| **Traditional Antivirus** | **Declining** | Less effective against adaptive threats |

**Key Insight:**  
Defense that **blocks or detects early** is more effective than **post-breach mitigation**.

---

## 🕒 **Era-Based Shift (2015–2025)**

| Era | Frequency | Severity | Explanation |
|-----|-----------|----------|-------------|
| **Pre-Pandemic** | Higher | Moderate | Stable systems and predictable workflows |
| **Pandemic (2020–2021)** | Lower | **High** | Rapid remote expansion → new vulnerabilities |
| **Recovery (2022–2023)** | Stabilizing | Declining | Security adaptation period |
| **Recent (2024–2025)** | Steady | Controlled | Matured cybersecurity posture |

**Key Insight:**  
Cybersecurity priorities shifted from **attack count** → to **impact control**.

---

## 🌐 **One-Line Summary**
**Modern cybersecurity focuses less on preventing attacks and more on minimizing impact when breaches occur.**

---

---

## 💼 Strategic Recommendations

*Based on findings from this analysis — actionable directions for security and business teams.*

**1. Prioritise patch management and phishing training over perimeter tools**
Unpatched software and human behaviour account for the majority of exploited vulnerabilities in this dataset. Organisations investing heavily in firewalls while neglecting update cycles and employee training are addressing the symptom, not the cause. Automated patch scheduling and quarterly phishing simulation programmes would close the highest-volume attack vectors first.

**2. Healthcare and Education sectors need dedicated cybersecurity budgets**
These two industries show disproportionately high user exposure relative to their typical security investment. Healthcare's zero-downtime dependency makes it uniquely vulnerable to ransomware leverage. A minimum security baseline — including offline backups and access segmentation — should be treated as operational necessity, not optional spend.

**3. Re-evaluate VPN-dependent remote access architecture**
VPN and early AI detection systems showed the highest financial losses during the pandemic period, when remote work scaled rapidly. Organisations still relying primarily on VPN infrastructure should assess a Zero Trust Network Access (ZTNA) model, which limits lateral movement even after initial breach.

**4. Shift incident response KPIs from frequency to severity**
The era analysis shows incident frequency is stabilising, but impact severity remains the critical variable. Security teams should track **mean financial loss per incident** and **mean resolution time** as primary KPIs — not just total incident count — to reflect the modern threat landscape accurately.


---

## 🛠️ Tech Stack
| Tool | Purpose |
|------|---------|
| **Python (Pandas, NumPy)** | Data Cleaning & Feature Engineering |
| **Matplotlib / Plotly** | Data Visualization |
| **SciPy 📈** | Statistical Validation (Regression, ANOVA, Correlation) |
| **Jupyter Notebook** | Analysis & Documentation |

---
