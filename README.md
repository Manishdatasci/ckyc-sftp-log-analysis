# 📊 CKYC SFTP Log Analysis

## 🔍 Overview
This project analyzes SFTP connection logs from a CKYC (Central Know Your Customer) system to identify failure patterns, diagnose system issues, and evaluate their impact on customer onboarding.

The goal is to uncover key insights from log data and propose actionable improvements to enhance system reliability and performance.

---

## 🎯 Objectives
- Analyze SFTP logs to detect failure trends  
- Identify root causes of system errors  
- Evaluate impact on users and system performance  
- Provide data-driven recommendations  

---

## 📁 Dataset Description
The dataset consists of SFTP log records containing:
- Timestamp of requests  
- Error types (e.g., PermissionDenied, TimeoutError)  
- Success/Failure status  
- Customer identifiers  

---

## 🛠️ Key Steps Performed

### 1. Data Cleaning
- Standardized column names  
- Converted timestamps into datetime format  
- Handled missing values  
- Removed inconsistencies  

### 2. Exploratory Data Analysis (EDA)
- Calculated failure rates over time  
- Analyzed error distribution  
- Compared system behavior before and after incident  

### 3. Feature Engineering
- Extracted date and time-based features  
- Grouped logs for trend analysis  

---

## 📉 Key Insights

- A **major spike in failure rate** was observed around mid-February, indicating a system-wide outage  
- Before the incident, most failures were due to **PermissionDenied errors (configuration issues)**  
- After the incident, **Timeout and connection errors increased**, suggesting system instability  
- Simultaneous failures across users indicate a **centralized system failure**  
- High request volume during failures suggests **retry storm behavior**, increasing system load  

---

## ❗ Key Issues Identified
- Configuration-related access errors  
- System-wide outage during peak period  
- Uncontrolled retry mechanism  
- Lack of real-time monitoring  

---

## 💼 Business Impact
- Delays in customer onboarding  
- Increased system load and instability  
- Potential SLA breaches  
- Poor user experience  

---

## 🚀 Recommendations
- Implement real-time monitoring and alert systems  
- Introduce pre-validation checks to reduce errors  
- Apply exponential backoff retry mechanism  
- Monitor infrastructure metrics (CPU, memory, latency)  
- Enable customer-level tracking for better debugging  

---

## 🧠 Conclusion
The analysis highlights a critical system failure that evolved from configuration issues to infrastructure instability. Implementing monitoring and optimized retry strategies can significantly improve system performance and reliability.

---

## 🛠️ Tech Stack
- Python  
- Pandas  
- Matplotlib / Seaborn  
- Jupyter Notebook  

---
