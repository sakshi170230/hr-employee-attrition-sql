SELECT COUNT(*) AS total_employees FROM hr_employee_data;
SELECT COUNT(*) AS attrition_count
FROM hr_employee_data
WHERE Attrition = 'Yes';
SELECT 
    ROUND(100.0 * SUM(CASE WHEN Attrition = 'Yes' THEN 1 ELSE 0 END) / COUNT(*), 2) AS attrition_rate
FROM hr_employee_data;
SELECT Department, COUNT(*) AS total, 
    SUM(CASE WHEN Attrition = 'Yes' THEN 1 ELSE 0 END) AS attrition_count
FROM hr_employee_data
GROUP BY Department;
SELECT JobRole, ROUND(AVG(MonthlyIncome), 2) AS avg_income
FROM hr_employee_data
GROUP BY JobRole;
