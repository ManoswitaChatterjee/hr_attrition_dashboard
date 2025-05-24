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

_______________________________________________________________________________________________________________________________________________________________________________________________

## Dashboard 1 - HR ATTRITION DASHBOARD
### KPIs 

![Screenshot_35](https://github.com/user-attachments/assets/7a45cc5c-dae2-4e65-9fa0-60c090e6843f)


1. **Current Employees -** This is the total number of employees curerently employed by the company.  
   **Formula :** ``` Total employees = IF ISNULL([Exit Date]) THEN 1 ELSE 0 END ```
   
2. **Total Attrition -** This shows the number of employeed attrited by the company.  
   **Formula:** ``` Attrited employees = IF NOT ISNULL([Exit Date]) THEN 1 ELSE 0 END ```

3. **Attrition Rate -** This KPI shows the percentage of people attrited from the overall company employee strength.  
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

#### _Employee Gender ratio_ 
This pie chart shows the percenatge plus the numbers of the employee division w.r.t to gender amidst the current working employees after attrition. In here we can clearly see that there is a significantly larger female employee population in the company at 55.86%.

#### _Attritition rate / Dept_
It shows details of number of attrition and retention distributed across all 6 departments plus department wise attrition rate as well. From this we can see that the highest attrition has taken place in 'Executive Office' with an attrition rate of 66.67%.

#### _Attrition rate / Business Unit_
This shows a similar details like the previous visualization but distributed among the various Business units of the company.

#### _Employee Performance across Dept_
This visuallization shows the existing employee performance across departments with Production team not only having the highest employee count but also having the most eomployees performing decent with their performance being under "Fully Meets"

#### _Current Employee Count / Business Unit_
It shows the top 5 Business units with the most employee count after attrition with CCDR leading at 169 employees. 

### Filters

![Screenshot_37](https://github.com/user-attachments/assets/394e3338-f8e8-4516-8130-53eda144ae5c)

a. **Gender -** To filter gender wise data.  
b. **Department -** To filter data according to departments.  
c. **Business Unit -** To filter data according to various Business units.  
d. **Division -** To filter data based on employee designations.  
e. **State -** To filter state(USA)-wise data.

_______________________________________________________________________________________________________________________________________________________________________________________________

## Dashboard 2 - RECRUITMENT DASHBOARD
### KPIs 

![Screenshot_36](https://github.com/user-attachments/assets/347905f7-aae1-4451-8f01-e7dea185dc92)


1. **Applicant Count -** This is the total number of people who applied for various roles in the company.  
   **Formula :** ``` Total applicants = COUNT([First Name]) ```
   
2. **Avg. Expected Salary -** This shows the average salary expectations of people who applied for the company reagrdless of the post they applied for.  
   **Formula:** ``` AVG(Desired Salary) ```

3. **Avg. Candidate Experience -** This KPI shows the average industry experience of the candidates who applied to the company.  
   **Formula:** ``` AVG(Years of Experience) ```

### Final Dashboard

![Screenshot_32](https://github.com/user-attachments/assets/7801687a-b039-4196-8db9-9dda63edcc94)


### Insight:
#### _Applicant Gender Ratio_
This pie chart shows the distribution of applicant's gender. Here we can see that most of the people who applied for the company are males but the difference from females or other gender people is not too big. 

#### _Applicant Qualification Details_ 
This visualization shows how many people among the applicants hold what qualification. We can see that there is a uniformity in the number of people who hold these 4 qualifications however most applicants hold Bachelor's Degree.

#### _Recruitment status_
It shows the distibution and status of applicants who have applied for jobs in the company distributed across 4 months. The different colos depict the status of applications like "Applied", "Interviewing" and aso on.

#### _Top 10 Desired Jobs_
This lists the top 10 jobs which has the most popularity among the applicants, i.e the jobs with the most applicants.

#### _Global Applicant Distribution_
This geographical visualization depits the total number of applicants from each country on a global scale. 

### Filters

![Screenshot_38](https://github.com/user-attachments/assets/b501e3ad-04f2-4f8a-a47b-f3d6da3ec39b)


a. **Country -** To filter data based on the country of applicants.  
b. **Education Level -** This filters data based on the highest eduactional qualification of the applicants.  
c. **Gender -** To filter data according to the Gender of applicants.  
d. **Status -** To filter data based on ethe status of their applications like "Applied", "In Review", "Interviewing" and so on.

_______________________________________________________________________________________________________________________________________________________________________________________________

## Dashboard 3 - APPLICANT DETAILS DASHBOARD
### Final Dashboard

![Screenshot_33](https://github.com/user-attachments/assets/95e5d9ef-da45-422b-98a6-4cac5b653387)


### Insight:
#### _Applicant Details_
This dashboard shows a details list of applicant details like their application ID, name, contact information, qualifications, address, years of experience and so on. 

The main purpose of this dashboard is to help recruiters figure out every detail of any applicant(s) through their id, name or so on from the filters given.

### Filters

![Screenshot_39](https://github.com/user-attachments/assets/a1c7218e-24d8-4d69-a288-4b39352a91da)



a. **Applicant ID -** To filter data based on the country of applicants. You can directly put the applicant ID in the box and search up the details.  
b. **Applicant Name -** This filters data based on the applicant name.  
c. **Application Date -** To filter data according to the Date of submitting application by the applicants.  
d. **Country -** To filter data based on the country of applicants.  
e. **Gender -** To filter data according to the Gender of applicants.  
f. **Application Status -** To filter data based on ethe status of their applications like "Applied", "In Review", "Interviewing" and so on.  
g. **Education Level -** This filters data based on the highest eduactional qualification of the applicants.  

_______________________________________________________________________________________________________________________________________________________________________________________________

### Conclusion 

The Hospital-dashboard provides a analysis of both hospital and patient data using the sample kaggle data set. The data is first cleaned and made appropriate for analysis and the vizualized into the dashboard using Power BI. The report highlighted essential performance metrics and uncovered valuable insights into hospital utilization, patient trends, and operational efficiency.

#### Recommendations and Key Takeaways

1. Unsurprisingly 65+ people are hospitalized for the most number of days and thus need more attention and regular check-ups.
2. Patients with 0-18 age have higher bill amount which may indicate that they are mostly hospitalized for some serious injury or immediate operations.
3. The KPI "Avg. Bill (Usd) indicates that a patient if hospitalized can expect an average bill amount of $25,540. Ofcourse this data varies hospital to hospital and can be checked using the "Hospital" filter.

This project helps visualize data and uncover insights, enabling both patients and hospitals to understand key metrics and support better decision-making for patient care and hospital operations.
