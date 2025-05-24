# HR ATTRITION DASHBOARD
It is an Interactive Tableau workbook that contains 3 dashboards viz. - Attrition Dashboard, Recruitment Dashboard and Applicant Dashboard to help analyze and understand over attrition, retention and recruitment metrics for the company to help management make better decisions.

Dashboard Link - https://public.tableau.com/app/profile/manoswita.chatterjee/viz/HRDashboard_17452484913400/AttritionDashboard 

### Introduction
This Dashboard helps to analyze and derive insights into employee attrition trends, departments affected, exit reasons, and key employee and applicant KPIs using synthetic workforce data.

### Goal 
1. **HR Attrition Dashboard:** Monitor and analyze employee turnover trends to identify high-risk areas, understand attrition and retention rates, and support data-driven retention strategies.
2. **Recruitment Dashboard:** Track hiring performance, open positions, applicant details and other KPIS to understand recruitment funnel efficiency to help optimize talent acquisition efforts.
3. **Applicant Details Dashboard:** Provide a detailed view of applicant profiles, application statuses, and qualification metrics to enhance candidate evaluation and selection.

### About the Dataset
1. The data used in this dashboard is from the "Employee/HR Dataset", available in Kaggle (https://www.kaggle.com/datasets/ravindrasinghrana/employeedataset?select=employee_data.csv)(https://www.kaggle.com/datasets/ravindrasinghrana/employeedataset?select=recruitment_data.csv)
3. This dataset contains fictional employee and recruitment data to derive insights into employee attrition trends, overall employee count, applicant geographical distribution, recruitment performance, employee gender ratio and so on.


## Dashboard 1 - HR ATTRITION DASHBOARD
### KPIs 

![Screenshot_35](https://github.com/user-attachments/assets/7a45cc5c-dae2-4e65-9fa0-60c090e6843f)


1. **Current Employees -** This KPI represents the total number of patients hospitalized in the hospital.
   **Formula :** SUM(Total employees) where
   ``` Total employees = IF ISNULL([Exit Date]) THEN 1 ELSE 0 END ```
   
3. **Total Attrition -** This KPI lists the average bill charged per person in the hospital i.e the avergae bill one can expect if being hospitalized.
   **Formula:** Average(Billing Amount)

2. **Attrition Rate -** This KPI lists the average bill charged per person in the hospital i.e the avergae bill one can expect if being hospitalized.
   **Formula:** Average(Billing Amount)

2. **Dept. Count -** This KPI lists the average bill charged per person in the hospital i.e the avergae bill one can expect if being hospitalized.
   **Formula:** Average(Billing Amount)

2. **Avg. Employee Rating -** This KPI lists the average bill charged per person in the hospital i.e the avergae bill one can expect if being hospitalized.
   **Formula:** Average(Billing Amount)
   

### Final Dashboard

![Screenshot_31](https://github.com/user-attachments/assets/f449c90b-eee2-4d1c-befc-393f62e44a42)

### Insight:
This Dashboard helps users to understand the Attrition and retention data of the company.

### Analysis
This dashboard aims to provide a detailed analysis of hospital performance and patient-related trends using key healthcare indicators.

The dashboard offers a broad understanding of patient admissions, hospitalization duration, and overall hospital metrices. By highlighting these areas, the report supports better understanding for people like - what bill they might expect, best insurance provider and so on.


















### Filters 
1. **Admission Year -** To filter patients data w.r.t the year they are admitted in the hospital.
2. **Age Group -** To filter data by patient age group.
3. **Medical Condition -** This filters patients by their diagnosed medical condition.
4. **Hospital -** To filter data by the hospital name.
5. **Insurance Provider -**  This filters data by the insurance provider patients are under.

![Screenshot_16](https://github.com/user-attachments/assets/30d03354-8718-4573-bb48-0824b0cf1cd3)


### Conclusion 

The Hospital-dashboard provides a analysis of both hospital and patient data using the sample kaggle data set. The data is first cleaned and made appropriate for analysis and the vizualized into the dashboard using Power BI. The report highlighted essential performance metrics and uncovered valuable insights into hospital utilization, patient trends, and operational efficiency.

#### Recommendations and Key Takeaways

1. Unsurprisingly 65+ people are hospitalized for the most number of days and thus need more attention and regular check-ups.
2. Patients with 0-18 age have higher bill amount which may indicate that they are mostly hospitalized for some serious injury or immediate operations.
3. The KPI "Avg. Bill (Usd) indicates that a patient if hospitalized can expect an average bill amount of $25,540. Ofcourse this data varies hospital to hospital and can be checked using the "Hospital" filter.

This project helps visualize data and uncover insights, enabling both patients and hospitals to understand key metrics and support better decision-making for patient care and hospital operations.
