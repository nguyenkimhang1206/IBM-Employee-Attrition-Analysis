# IBM Employee Attrition Analysis
# 1. Problem Statement

HR Analytics helps us with interpreting organizational data. It finds the people-related trends in the data and allows the HR Department to take the appropriate steps to keep the organization running smoothly and profitably. Attrition in a corporate setup is one of the complex challenges that the people managers and the HRs personnel have to deal with.

This is a fictional data set created by IBM data scientists.

**Goal** : Understand the employee attrition rate in the company and identify the factors that affect it.

# **2. Dataset Description**

This is a fictional data set created by IBM data scientists. The dataset is based on HR data collected by IBM, consists of 1,470 records, containing a rich set of features related to employees, including demographics, job role, work environment, and performance indicators. 

This dataset contains 35 columns and can be found [here](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset/code). The data dictionary is available [here](https://github.com/nguyenkimhang1206/IBM-Employee-Attrition-Analysis/blob/main/Data%20Dictionary%20of%20IBM%20Dataset.xlsx).

# 3. Insights Summary

### #1 Overview of attrition rate

- **Attrition rate in company:** The overall attrition rate in the company is 16.1% (236 employees).
  
![image](https://github.com/user-attachments/assets/c00fb06e-ed38-42fa-b049-d2f1addd45f5)


- **Attrition rate by department:** The Sales department has the highest attrition rate at 20.6%, followed by the HR department at 19%, with the R&D department having the lowest rate.
  
  ![image](https://github.com/user-attachments/assets/ddc8be76-82c6-47c6-9229-b7f8c999e0c4)
  
- **Attrition rate by job role:**

  Within the Sales department, the Sales Representative position has an attrition rate of nearly 40%, which is double that of the Sales Executive position.

  In the R&D department, the Laboratory Technician role has the highest attrition rate about 24%, followed by the Research Scientist role.
  
  ![image](https://github.com/user-attachments/assets/a9844533-b2ad-473a-b9c2-48e7b098645c)
### #2 Compensation Issue

- **Monthly Income**: Employees who stay with the company generally have higher incomes compared to those who leave. Specifically, 50% of employees who have left earn $3,200 or less, while only 25% of employees who remain earn $3,200 or less. This suggests that higher-income employees are more likely to stay with the company.
  
  ![image](https://github.com/user-attachments/assets/8f4943ac-a42a-46ec-b9e7-a6dd4760b3ad)
  
### #3 Management Issue

- **Years With Current Manager**: Employees who remain with the company generally have more tenure with their current manager. Specifically, 50% of employees who have left have been with their current manager for 2 years or less, while 50% of employees who stay have been with their manager for 3 years or less. This could imply that stronger relationships with managers contribute to higher employee retention.
  
  ![image](https://github.com/user-attachments/assets/4685debf-ddca-42d1-bb26-2593a2207cbb)

### #4 Work Environment Issues

- **Environment Satisfaction**: Employees who are dissatisfied with their work environment are more likely to leave the company. As environment satisfaction improves, attrition rates decrease, with employees who score 4 experiencing the lowest attrition. This pattern underscores the importance of a positive work environment in retaining employees. 
  
![image](https://github.com/user-attachments/assets/737888ea-e147-419f-ba40-8f17a831b086)

- **Job Satisfaction**: Employees with the lowest job satisfaction (score of 1) exhibit the highest attrition rates. This indicates that employees who are highly dissatisfied with their jobs are more likely to leave the company. Conversely, as job satisfaction increases, attrition rates decrease, with employees who score 4 on job satisfaction showing the lowest attrition rates. This trend underscores the critical role of job satisfaction in employee retention.
  
  ![image](https://github.com/user-attachments/assets/4cdae7f2-03a9-491b-8026-02d568501a0a)

- **Relationship Satisfaction**: Employees with the lowest relationship satisfaction (score of 1) have the highest attrition rates. This suggests that employees who are highly dissatisfied with their relationships at work are more likely to leave the company. As relationship satisfaction improves, attrition rates decrease. This indicates that positive relationships at work are strongly associated with higher employee retention. 
  
  ![image](https://github.com/user-attachments/assets/c5f621df-0927-409f-b83e-4fa577efe982)
  
- **Over Time**: Employees who work overtime exhibit the high attrition rate, at 30.5%, triple that of those who don't. This suggests that employees required to work overtime are more likely to leave the company compared to those who do not. The higher attrition rate among overtime workers may indicate that excessive work hours contribute to increased employee dissatisfaction or burnout.
  
![image](https://github.com/user-attachments/assets/b95b2b5b-3094-48af-b140-6dcc5b223415)

### #5 Work Experience Factors

- **Years At Company**: Employees who stay with the company generally have more tenure compared to those who leave. Specifically, 50% of employees who have left have been with the company for 3 years or less, while 50% of employees who remain have been with the company for 6 years or less. The higher median tenure for employees who stay suggests that longer company tenure is associated with lower attrition rates, implying that employees with more years at the company are more likely to stay.
  
![image](https://github.com/user-attachments/assets/d92a4575-4257-45a0-8066-b451c77dd1ed)

- **Years In Current Role**: Employees who remain with the company generally hold their current role for longer periods compared to those who leave. Specifically, 50% of employees who have left have been in their role for 2 years or less, while 50% of employees who stay have held their role for 3 years or less. The higher median for employees who remain suggests that longer tenure in the same role is associated with lower attrition rates, implying that employees who have been in their current role longer are more likely to stay with the company.
  
![image](https://github.com/user-attachments/assets/55a0d117-54b1-46e5-ad24-95568853982d)

- **Total Working Years**: Employees who remain with the company tend to have more total working experience compared to those who leave. Specifically, 50% of employees who have left have 7 years or less of work experience, while 50% of those who stay have 10 years or less. Additionally, the wider spread in total working years for the non-attrition group suggests that more experienced employees are more likely to stay with the company. This implies that longer overall career experience is associated with lower attrition rates.
  
  ![image](https://github.com/user-attachments/assets/50281294-94e8-444a-a6a8-d239852d5097)
  
    
- **Job Involvement**: Employees who are less engaged or involved in their work are more likely to leave the company. As job involvement increases, attrition rates decrease, with employees who score 4 on job involvement experiencing the lowest attrition. This pattern indicates that higher levels of job involvement are associated with greater employee retention. Fostering higher engagement and involvement in the workplace could be a key strategy to reduce attrition, especially for employees with low job involvement.
  
![image](https://github.com/user-attachments/assets/f3748efb-07c8-4404-a498-ae26f2ceb8a6)

- **Job Level**: Employees who remain with the company generally occupy higher job levels compared to those who leave. Specifically, 50% of employees who have left are at job level 1, while 50% of employees who stay are at job level 2. The higher median job level for employees who stay suggests that more senior positions are associated with lower attrition rates, implying that employees in higher job levels are more likely to remain with the company.
  
  ![image](https://github.com/user-attachments/assets/fade8fea-fe8b-4da0-b56e-9a9c6b3abc10)
  
### #6 Personal Issue

- **Work Life Balance**: Employees with the lowest work-life balance (score of 1) have the highest attrition rate, indicating that poor work-life balance is a significant factor contributing to employees leaving the company. This suggests that employees who perceive a better work-life balance are more likely to stay with the company, while those facing work-life imbalance are at a higher risk of leaving. Improving work-life balance, particularly for those with a score of 1, could be an effective strategy to reduce attrition.
  
![image](https://github.com/user-attachments/assets/23f4b7eb-7ec3-4539-b02f-90eae2722f23)

- **Age**: Younger employees are more likely to leave the company, as 50% of employees who have left are 32 years old or younger, while 50% of employees who remain are 36 years old or younger. Additionally, the broader age range of employees who stay, with 75% being 43 years or younger, implies that older employees are more likely to stay with the company, while younger employees are at a higher risk of leaving. This could suggest that younger employees might have different expectations or face different challenges, which could be contributing to higher attrition in this group.
  
![image](https://github.com/user-attachments/assets/0b4b6497-55e5-4a6c-96e8-0efddeeb2542)

- **Distance From Home**: Employees who live farther from the workplace are more likely to leave the company, as 50% of employees who left live 9 km or farther from the workplace, compared to 50% of employees who stay, who live 7 km or less. Additionally, the wider range of commuting distances for employees who have left indicates that longer commutes could be a contributing factor to higher attrition rates. Improving flexibility or addressing commute-related challenges could help reduce attrition, particularly for employees who live farther away.
  
![image](https://github.com/user-attachments/assets/2258a4bc-fa26-49a5-899f-fe82b05051ee)

# 4. Conclusion

- The analysis reveals that several key factors influence employee attrition, including c**ompensation, management, work environment, work experience, and personal issues.** 

- Employees with **lower income, shorter tenure with their manager, less work experience, lower job involvement, and lower job levels** tend to leave.

- Additionally, **poor scores in environment, job, and relationship satisfaction, as well as high levels of overtime,** contribute to higher attrition rates, highlighting issues with the work environment. 

- Personal factors like **poor work-life balance, younger age, and proximity to the workplace** also play a role in employee turnover.

# 5. Recommendation

- Utilize the identified factors influencing employee attrition to **conduct a more detailed analysis of attrition reasons within each department and job rol**e. Specifically, focus on departments with high attrition rates, Sales and HR, as well as job roles with high turnover, including Sales Representatives and Laboratory Technicians. **Develop targeted strategies tailored to address the unique challenges faced by each department and role.**
- **Enhance the dataset** by incorporating additional variables such as the timing of attrition, reasons for departure (as indicated in exit surveys), and the impact of attrition (e.g., associated costs like hiring and training expenses). This will provide a comprehensive foundation for future analyses.
- Apply predictive modeling techniques to **assess which factors most significantly influence attrition and to forecast which employees are likely to leave**. This approach will help in developing proactive measures to improve retention.
