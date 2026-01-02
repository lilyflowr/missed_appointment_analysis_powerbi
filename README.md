# Reducing Missed Appointments in an Outpatient Clinic  
*A Healthcare Data Analytics Case Study*

![Dashboard Overview](screenshots/dashboard.png)
---

## Project Overview
Missed outpatient appointments negatively affect continuity of care, clinic efficiency, and resource utilization.  
This project analyzes outpatient appointment data to identify factors contributing to missed appointments and provides data-driven recommendations to improve appointment adherence.

Using **Excel for data preparation** and **Power BI for analysis and visualization**, I explored how waiting time, SMS reminders, patient demographics, appointment timing, and underlying medical conditions influence no-show behavior.

This case study reflects my background in healthcare and my transition into data analytics, focusing on practical insights rather than purely descriptive statistics.

---

## Business Problem
The outpatient clinic experienced a consistent decline in completed follow-up appointments over time, leading to underutilized appointment slots and disrupted patient care.

**Business Task:**  
Identify key factors associated with missed appointments and recommend actionable interventions to reduce no-show rates.

---

## Stakeholders
- Head of Hospital (primary decision maker)  
- Lead Doctor  
- Lead Nurse  
- Outpatient Operations Team  

---

## Dataset
**Source:** Medical Appointment No Shows (Brazil) – Kaggle  
🔗 https://www.kaggle.com/datasets/joniarroba/noshowappointments

**Size:**  
- 110,527 rows  
- 14 columns  

**Key Fields:**  
- Appointment scheduling and appointment dates  
- Patient demographics (age, gender)  
- SMS reminder indicator  
- Attendance outcome (missed vs attended)  
- Chronic condition indicators  

> Note: The dataset is anonymized and publicly available. While it is based on Brazilian outpatient data, the behavioral patterns analyzed are applicable to broader healthcare contexts.

---

## Tools & Skills
**Tools**
- Excel (data cleaning and preparation)  
- Power BI (data modeling, DAX, visualization)

**Skills Demonstrated**
- Exploratory Data Analysis (EDA)  
- DAX measure creation  
- Healthcare analytics  
- Business insight generation  
- Data visualization for decision-making  

---

## Data Cleaning & Preparation
Data preparation was performed in Excel before loading into Power BI.

Key steps included:
- Data integrity checks  
- Duplicate detection and removal  
- Data type validation  
- Standardization of date and time fields  
- Transformation of the MissedAppointment column to Boolean (1 = missed, 0 = attended)  
- Splitting datetime fields into separate date and time columns  
- Removal of default appointment time values (00:00:00)

---

## Key Metrics (DAX Measures)
The following core metrics were created in Power BI:

- **Total Appointments**  
- **Number of Missed Appointments**  
- **Missed Appointment Rate (%)**

These measures formed the foundation for all analysis and visualizations.

---

## Analysis & Visualizations

### 1. Overall Missed Appointment Rate
![KPI Cards](screenshots/missed_appointment_rate.png)

Approximately **20% of all outpatient appointments were missed**, highlighting a significant operational challenge.

---

### 2. SMS Reminders vs Missed Appointments
![SMS Analysis](screenshots/sms_vs_missed.png)

Appointments that received SMS reminders showed a higher missed appointment rate. Further analysis revealed that SMS reminders were often used for higher-risk appointments rather than being a direct cause of missed visits.

---

### 3. Waiting Time Impact
![Waiting Time Analysis](screenshots/waiting_time.png)

Waiting time between scheduling and appointment date was the strongest predictor of missed appointments. Longer waiting periods were associated with significantly higher no-show rates, even when SMS reminders were sent.

---

### 4. Age Group Analysis
![Age Group Analysis](screenshots/age.png)

Patients aged **18–35** had the highest missed appointment rates, while patients aged **56+** were the most consistent attendees.

---

### 5. Underlying Medical Conditions
![Underlying Conditions](screenshots/underlying_condition.png)

Patients without chronic conditions were more likely to miss appointments compared to those managing ongoing health issues. Alcoholism was associated with the highest missed appointment rate among the conditions analyzed.

---

## Key Insights
- Waiting time is the strongest driver of missed appointments.  
- SMS reminders alone are insufficient for long-wait appointments.  
- Younger patients are more likely to miss appointments.  
- Patients with chronic conditions are generally more consistent attendees.  
- Behavioral health conditions may require additional scheduling support.

---

## Recommendations
- Reduce appointment lead times where operationally possible.  
- Flag long-wait appointments for proactive follow-up.  
- Apply differentiated engagement strategies for younger patients.  
- Provide targeted support for patients with behavioral health conditions.  

---

## Project Deliverables
- Power BI dashboard (visual analysis)  
- Medium article with full narrative case study  
- GitHub documentation and assets  

🔗 **Medium article:** *(https://ibinaboadiela.medium.com/why-patients-miss-appointments-what-110-000-hospital-records-taught-me-about-missed-appointments-931162d24106)*

---

