# IBM Employee Attrition Analysis

# 1. Problem Statement

HR Analytics helps us with interpreting organizational data. It finds the people-related trends in the data and allows the HR Department to take the appropriate steps to keep the organization running smoothly and profitably. Attrition in a corporate setup is one of the complex challenges that the people managers and the HRs personnel have to deal with.

This is a fictional data set created by IBM data scientists.

**Goal** : Understand the employee attrition rate in the company and identify the factors that affect it.

# **2. Dataset Description**

The data consists of 1,470 records, including information about employee demographics, satisfaction scores, income, and other details.

This dataset contains 35 columns and can be found [here](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset/code). The data dictionary is available [here](https://github.com/nguyenkimhang1206/IBM-Employee-Attrition-Analysis/blob/main/Data%20Dictionary%20of%20IBM%20Dataset.xlsx).

# 3. Insights Summary

### #1 Overview of attrition rate

- Attrition rate in company: The overall attrition rate in the company is 16.1% (236 employees). The Sales department has the highest attrition rate at 20.6%, followed by the HR department at 19%, with the R&D department having the lowest rate.

![image.png](image.png)

- Attrition rate by department: Within the Sales department, the Sales Representative position has an attrition rate of nearly 40%, which is double that of the Sales Executive position.
    
    ![image.png](image%201.png)
    
- Attrition rate by job role: In the R&D department, the Laboratory Technician role has the highest attrition rate at 23%, followed by the Research Scientist role.
    
    ![image.png](image%202.png)
    

### #2 Compensation

- MonthlyIncome

![image.png](image%203.png)

The box plot indicates that employees who stay with the company generally have higher incomes compared to those who leave. Specifically, **50%** of employees who have left earn **$3,200** or less, while only **25%** of employees who remain earn **$3,200** or less. **This suggests that higher-income employees are more likely to stay with the company.**

### #3 Management

- YearsWithCurrManager

![image.png](image%204.png)

The box plot indicates that employees who remain with the company generally have more tenure with their current manager. Specifically, **50%** of employees who have left have been with their current manager for **2 years or less**, while **50%** of employees who stay have been with their manager for **3 years or less**. The longer tenure of employees who remain suggests that employees who have a longer relationship with their manager are more likely to stay with the company. This could imply that stronger relationships with managers contribute to higher employee retention.

### #4 Work Environment Issue

- EnvironmentSatisfaction  (**Factor)**

![image.png](image%205.png)

This suggests that employees who are dissatisfied with their work environment are more likely to leave the company. As environment satisfaction improves, attrition rates decrease, with employees who score **4** experiencing the lowest attrition. This pattern underscores the importance of a positive work environment in retaining employees. Addressing environmental factors, particularly for those with low satisfaction, could help in reducing attrition rates and improving overall employee retention.

- JobSatisfaction  (**Factor)**

![image.png](image%206.png)

The stacked bar chart depicting attrition rates by job satisfaction levels (rated from 1 to 4) highlights a significant trend: employees with the lowest job satisfaction (score of **1**) exhibit the highest attrition rates. This indicates that employees who are highly dissatisfied with their jobs are more likely to leave the company. Conversely, as job satisfaction increases, attrition rates decrease, with employees who score **4** on job satisfaction showing the lowest attrition rates. This trend underscores the critical role of job satisfaction in employee retention. Enhancing job satisfaction, particularly for those with the lowest ratings, could be a key strategy in reducing attrition and improving employee retention.

- RelationshipSatisfaction (**Factor)**

![image.png](image%207.png)

The stacked bar chart illustrating attrition rates by relationship satisfaction levels (rated from 1 to 4) reveals a clear pattern: employees with the lowest relationship satisfaction (score of **1**) have the highest attrition rates. This suggests that employees who are highly dissatisfied with their relationships at work are more likely to leave the company. As relationship satisfaction improves, attrition rates decrease, with employees scoring **4** showing the lowest attrition rates. This indicates that positive relationships at work are strongly associated with higher employee retention. Addressing issues related to workplace relationships, particularly for those with low satisfaction, could be a crucial strategy in reducing overall attrition and enhancing employee retention.

- OverTime  (**factor**)

![image.png](image%208.png)

The stacked bar chart comparing attrition rates by overtime status reveals that employees who work overtime exhibit the highest attrition rate, at **30.5%**. This suggests that employees who are required to work overtime are more likely to leave the company compared to those who do not work overtime. The higher attrition rate among overtime workers may indicate that excessive work hours could be contributing to increased employee dissatisfaction or burnout. Addressing the reasons behind the high attrition among employees who work overtime and finding ways to manage or reduce overtime could be essential strategies for improving retention and overall employee well-being.

### #5 Other Job Factors

- JobInvolvement

![image.png](image%209.png)

employees who are less engaged or involved in their work are more likely to leave the company. As job involvement increases, attrition rates decrease, with employees who score **4** on job involvement experiencing the lowest attrition. This pattern indicates that higher levels of job involvement are associated with greater employee retention. Fostering higher engagement and involvement in the workplace could be a key strategy to reduce attrition, especially for employees with low job involvement.

- JobLevel
    
    ![image.png](image%2010.png)
    
    Employees who remain with the company generally occupy higher job levels compared to those who leave. Specifically, **50%** of employees who have left are at job level **1**, while **50%** of employees who stay are at job level **2**. The higher median job level for employees who stay suggests that more senior positions are associated with lower attrition rates, implying that employees in higher job levels are more likely to remain with the company.
    

### #6 Work Experience

- YearsAtCompany

![image.png](image%2011.png)

This indicates that employees who stay with the company generally have more tenure compared to those who leave. Specifically, **50%** of employees who have left have been with the company for **3 years or less**, while **50%** of employees who remain have been with the company for **6 years or less**. The higher median tenure for employees who stay suggests that longer company tenure is associated with lower attrition rates, implying that employees with more years at the company are more likely to stay.

- YearsInCurrentRole

![image.png](image%2012.png)

Employees who remain with the company generally hold their current role for longer periods compared to those who leave. Specifically, **50%** of employees who have left have been in their role for **2 years or less**, while **50%** of employees who stay have held their role for **3 years or less**. The higher median for employees who remain suggests that longer tenure in the same role is associated with lower attrition rates, implying that employees who have been in their current role longer are more likely to stay with the company.

- TotalWorkingYears

![image.png](image%2013.png)

Employees who remain with the company tend to have more total working experience compared to those who leave. Specifically, **50%** of employees who have left have **7 years or less** of work experience, while **50%** of those who stay have **10 years or less**. Additionally, the wider spread in total working years for the non-attrition group suggests that more experienced employees are more likely to stay with the company. This implies that longer overall career experience is associated with lower attrition rates.

- NumCompaniesWorked

![image.png](image%2014.png)

Employees who leave the company tend to have worked for fewer companies overall, with **50%** of them having worked for only **1 company**. In contrast, **50%** of employees who stay have worked for **2 companies or less**, and their overall range of prior employers is narrower. The higher number of previous companies worked for among employees who stay suggests that those with more diverse work experiences may be more likely to remain with the company, possibly because they have gained broader experience in different environments.

# #8 Personal Issue

- WorkLifeBalance

![image.png](image%2015.png)

 Employees with the lowest work-life balance score of **1** have the highest attrition rate, indicating that poor work-life balance is a significant factor contributing to employees leaving the company. This suggests that employees who perceive a better work-life balance are more likely to stay with the company, while those facing work-life imbalance are at a higher risk of leaving. Improving work-life balance, particularly for those with a score of **1**, could be an effective strategy to reduce attrition.

- Age ****

![image.png](image%2016.png)

younger employees are more likely to leave the company, as **50%** of employees who have left are **32 years or younger**, while **50%** of employees who remain are **36 years or younger**. Additionally, the broader age range of employees who stay, with **75%** being **43 years or younger**, implies that older employees are more likely to stay with the company, while younger employees are at a higher risk of leaving. This could suggest that younger employees might have different expectations or face different challenges, which could be contributing to higher attrition in this group.

- DistanceFromHome

![image.png](image%2017.png)

employees who live farther from the workplace are more likely to leave the company, as **50%** of employees who left live **9 km or farther** from the workplace, compared to **50%** of employees who stay, who live **7 km or less**. Additionally, the wider range of commuting distances for employees who have left indicates that longer commutes could be a contributing factor to higher attrition rates. Improving flexibility or addressing commute-related challenges could help reduce attrition, particularly for employees who live farther away.

# 4. Conclusion

The analysis reveals that employees who left the company often had lower salaries, shorter tenures with their current manager, and lower job levels. They also had fewer years with the company, less experience in their current role, and a lower number of previous employers. Additionally, younger employees and those living fartherto the company were more likely to leave. Key dissatisfaction indicators included low scores in environment satisfaction, job satisfaction, relationship satisfaction, job involvement, and work-life balance. Employees who worked overtime also had higher attrition rates. These insights suggest that addressing compensation, improving job and relationship satisfaction, enhancing career development opportunities, and managing overtime effectively could help reduce employee turnover.

# 5. Recommendation

- Utilize the identified factors influencing employee attrition to conduct a more detailed analysis of attrition reasons within each department and job role. Specifically, focus on departments with high attrition rates, Sales and HR, as well as job roles with high turnover, including Sales Representatives and Laboratory Technicians. Develop targeted strategies tailored to address the unique challenges faced by each department and role.
- Enhance the dataset by incorporating additional variables such as the timing of attrition, reasons for departure (as indicated in exit surveys), and the impact of attrition (e.g., associated costs like hiring and training expenses). This will provide a comprehensive foundation for future analyses.
- Apply predictive modeling techniques to assess which factors most significantly influence attrition and to forecast which employees are likely to leave. This approach will help in developing proactive measures to improve retention.