# 📊 Call Center Dashboard Analysis

This repository contains a complete **Call Center Analytics Project** powered by **SQL + Power BI + Reporting**.  
The project demonstrates end-to-end data analysis: from extracting insights using SQL, to building an interactive dashboard in Power BI, and finally delivering a strategic consulting-style report.

---

## 🚀 Project Overview
- **Dataset:** 500 call center records (calls, durations, issues, resolutions, satisfaction, agents, companies).  
- **Tools Used:**  
  - SQL (Data extraction, cleaning, KPI generation)  
  - Power BI (Interactive dashboard)  
  - Word / Reporting (Strategic insights & recommendations)  

The goal is to **analyze call center performance** and provide **actionable insights** to improve customer satisfaction, operational efficiency, and decision-making.

---

## 🎯 Objectives
1. Identify trends in call volumes and issue types.  
2. Evaluate resolution effectiveness and escalation patterns.  
3. Measure customer satisfaction levels (CSAT).  
4. Assess agent performance.  
5. Provide short- and long-term recommendations for improvement.  

---

## 📌 Core Insights
- **Call Volumes:** Payment (115) and Service Requests (108) dominate (~45% of calls).  
- **Call Duration:** Complaints take longest (30.4 mins); Account Info shortest (27.7 mins).  
- **Resolution Rates:** Only 33.6% resolved; 35.8% unresolved; 30.6% escalated.  
- **Customer Satisfaction:** Average CSAT = 3 (moderate satisfaction).  
- **Agent Performance:** Some agents achieve higher CSAT (e.g., Antonio Johnson, Bruce Carey).  
- **Workload Patterns:** 72% of calls occur on weekdays → staffing imbalance.  

---

## ⚠️ Problems Identified
1. High unresolved & escalated calls reduce customer trust.  
2. Payment-related issues dominate, suggesting weak self-service/payment processes.  
3. Long complaint handling times.  
4. CSAT stagnates at 3/5 (moderate satisfaction only).  
5. Agent performance inconsistencies.  

---

## 🛠️ Strategic Recommendations

### Short-Term (0–6 months)
- Improve **First Call Resolution (FCR)** with better scripts & knowledge base.  
- Reduce payment-related calls by enhancing **self-service systems**.  
- Provide **targeted agent training** using top performers as benchmarks.  
- Apply stricter escalation protocols.  

### Long-Term (6–18 months)
- Deploy **AI chatbots/automation** for repetitive issues.  
- Launch structured **customer feedback loop** (post-call surveys + sentiment analysis).  
- Redesign **staffing model** to align with weekday peak demand.  
- Conduct **root-cause analysis** for recurring complaints.  
- Introduce **CSAT-linked incentive programs** for agents.  

---

## 📂 Repository Structure

```
call-center-analysis/
│── README.md                     # Project overview (this file)
│── sql/                           # SQL scripts used for analysis
│    └── call_center_queries.sql
│── powerbi/                       # Power BI dashboard file
│    └── call_center_dashboard.pbix
│── report/                        # Strategic report
│    └── Call_Center_Dashboard_Analysis.docx
│── data/                          # Dataset (if shareable)
     └── calls_dataset.csv
```

---

## 📊 Dashboard Preview
<img width="472" height="269" alt="Page 1" src="https://github.com/user-attachments/assets/f37251d9-cbe4-4bb0-8933-26e47165e386" />
<img width="470" height="268" alt="Page 2" src="https://github.com/user-attachments/assets/a802b1f8-2a20-4e34-b6c9-afade0efca0e" />
<img width="473" height="262" alt="Page 3" src="https://github.com/user-attachments/assets/9c671bd3-5ed7-4255-85bb-ee5e0e66ab6e" />

---

## 📑 Report
The full **consulting-style report** is available in:  
`/report/Call center report.docx`  

It includes:  
- Executive summary  
- Core insights  
- Identified problems  
- Strategic recommendations (short & long term)  
- SQL-backed methodology appendix  

---

## 🔍 Methodology

This project followed a structured workflow:  

1. **SQL Queries** → Extract KPIs (calls, durations, escalations, CSAT, etc.)  
2. **Power BI Dashboard** → Visualize trends, patterns, and distributions.  
3. **Strategic Report** → Translate analytics into **business insights & recommendations**.  

Example SQL Queries:  
```sql
-- Total calls
SELECT COUNT(*) FROM `call center dataset`;

-- Average call duration
select avg(`call duration (mins)`) as average_call_duration
from call_center_dataset

-- Calls by issue type
select `issue type`, count(*) as issue_count
from call_center_dataset
group by `issue type`;

-- Escalations vs Resolutions
SELECT `resolution status`, COUNT(*)
FROM  `call center dataset` GROUP BY `resolution status`;

-- Weekday vs Weekend calls
select * from call_center_dataset
where dayofweek(`call date`)=1 or dayofweek(`call date`)=7;

-- CSAT per agent
select `agent name`,avg(`customer satisfaction score`) as highest_call_per_agent
from call_center_dataset
group by `agent name`;
```

---

## 📌 Key Learning Outcomes
- Using **SQL** to extract and analyze operational data.  
- Building professional dashboards with **Power BI**.  
- Writing **data-driven reports** for business stakeholders.  
- Bridging the gap between **technical results** and **strategic recommendations**.  

---

## 📧 Contact
Author: *Odewusi Kolawole*  
- LinkedIn: https://www.linkedin.com/in/kolawole-odewusi-940438231
- GitHub: https://github.com/WoleTheAnalyst
- Email: Kolawoleodewusi@gmail.com 

---

