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


1. **Current Employees -** This is the total number of employees curerently employed by the company.
   **Formula :** ``` Total employees = IF ISNULL([Exit Date]) THEN 1 ELSE 0 END ```
   
2. **Total Attrition -** This shows the number of employeed attrited by the company.
   **Formula:** ``` Attrited employees = IF NOT ISNULL([Exit Date]) THEN 1 ELSE 0 END ```

3. **Attrition Rate -** This KPI the percentage of people attrited from the overall company employee strength.
   **Formula:** ``` Attrition rate = ([Attrition] / [Employee Count]) ``` and
    ``` Attrition = count(IF NOT ISNULL([Exit Date]) THEN [Employee Full Name] END) ```

4. **Dept. Count -** This KPI lists the total number of departments in the company.
   **Formula:** ``` Total Dept = COUNTD([Department Type]) ```

5. **Avg. Employee Rating -** This displays the average ratings of all the current working out of 5.
   

### Final Dashboard

![Screenshot_31](https://github.com/user-attachments/assets/f449c90b-eee2-4d1c-befc-393f62e44a42)

### Insight:
#### _Distribution of Type of Employees working_
This visualization helps to show the percentage distribution and count of all the current employees' employeement type i.e. how many are full-time, part-time and temporary employees.

#### Employee Gender ratio 
This pie cahrt shows the percenatge plus the numbers of the employee division w.r.t to gender amidst the current working employees after attrition. In here we can clearly see that there is a significantly larger female employee population in the company at 55.86%.

#### Attritition rate / Dept
It shows details of number of attrition and retention distributed across all 6 departments plus department wise attrition rate as well. From this we can see that the highest attrition has taken place in 'Executive Office' with an attrition rate of 66.67%.

#### Attrition rate / Business Unit
This shows a similar details like the previous visualization but distributed among the various Business units of the company.

#### Employee Performance across Dept
This visuallization shows the existing employee performance across departments with Production team not only having the highest employee count but also having the most eomployees performing decent with their performance being under "Fully Meets"

#### Current Employee Count / Business Unit
It shows the top 5 Business units with the most employee count after attrition with CCDR leading at 169 employees. 















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
