# HEALTH-CHECK-ANALYSIS
This report conducts a health check of gender equity in terms of salary. Given one key question and the use of data storytelling to present the findings, insights and recommendations.

### Overview 
This analysis is vital for identifying potential salary disparities and promoting gender equality in the
workplace.

Two datasets will be used to conduct this analysis such as the employees information and employees performance. The analysis and tools used in this report is the Structured Query Language and the Tableau visualization tool we seek to uncover insights that will inform actions and recommendations to promote gender equity in salary distribution.

### Key Question 
- "is there a correlation between salary and gender"
The task involved examining whether there is a correlation between an employee's annual salary and their gender.

### Data Sources 
-  Employee infomation dataset 
-  Employee perfomance dataset

### Tools 
-  SQL LITE for data analysis 
- Tableau for data visualization

### SQL Analysis 

```sql
SELECT AVG(Employee_Performance.Annual_Salary) AS avg_annual_salary, Employee_Information.gender 
FROM Employee_Performance 
JOIN Employee_Information 
ON Employee_Performance.Employee_ID = Employee_Information.Employee_ID 
GROUP BY Employee_Information.gender;
```

### Tableau Visualization 
The diagram below reflect the relationship between annual salary and gender. From our key question,  the diagram explains that the annual salary of all the employees varies differently across the three identified genders. For female employees, the annual salary is around £79,487 annually and although male employees and Non-Binary employees figures seem closely equal, there is still a difference incurred by male employees. , making the Non-Binary employees the highest paid.

### Recommendations 
- Conduct a comprehensive review of our salary structure and policies to ensure fairness and transparency in compensation practices. 

- Implement measures to mitigate gender bias in salary negotiations and performance evaluations. 

- Provide training and education on gender equity and unconscious bias for all employees, especially those involved in salary decisions.

- Regularly monitor and analyze salary data to track progress and identify any ongoing disparities. 

- Foster a culture of inclusivity and diversity within the organization to create an environment where all employees feel valued and empowered. 

- Further analysis could be conducted to explore other aspects of equity, such as promotion rates and performance ratings in relation to gender

Full project [Download here](https://submissions.cloudfront.entrylevel.net/files/submission/bdbdb24c-a7bf-4256-ac21-28d3235d3a42.pdf?_gl=1*to61wi*_ga*MTcwNTEwNTkwMi4xNzMwNDY0OTUw*_ga_8RTQ11GGMX*MTczOTQ2OTAyMC40LjEuMTczOTQ3MTkzOS41OS4wLjA.)
