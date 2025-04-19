# Data_Cleaning_Power_Query

Analysis were based on the following questions:

1. Which job titles offer the highest salaries?
2. Which states has the highest compensations?
3. What is the size of the companies that pays the best salary?
4. What are the states and Job titles that pay the highest salary?

Data Cleaning and transformation were performed before Data Analysis.

1. Checked for duplicates; No duplicates
2. Changed 'Salary Estimate' column to actual salaries removing text characters in brackets.
3. Created two new columns 'Min Salary' and 'Max Salary' for minimum and maximum salary ranges.
4. Renaming similar job titles to a single type and creating a new column 'Role title' and changed type to text.
5. Filtering invalid values in 'Size' column.
6. Created a new column 'Location Corrected' as the existing column had null values for city in some columns.
7. Split the column 'Location Corrected' into two namely 'City' and 'State' and replaced the value 'Anne Arundel' in 'State' column with "MD' for Maryland state.
8. Created a duplicate query 'Salary by Role Title' to analyse the to analyse the minimum and maximum salaries based on role title.
9. Changed the type of Minimum and Maximum salary to currencies and multiplied with thousand.
10. Grouped Min and Max salaries based on Role Title to get overall counts 
11. Created a reference query 'Salary by Company Size' to analyse the minimum and maximum salaries based on company size.
12. Imported state mapping file and state abbreviations were mapped to the 'State' column in the DS_jobs_before_cleaning file.
13. Trimmed blanks in 'State' column.
14. Created a new duplicate query 'Salary by State' to analyse the minimum and maximum salaries based on state.
15. Created a new reference query 'Salary by State and Role Title' to analyse the minimum and maximum salaries based on state and role type.


Once cleaned, the data began to tell some fascinating stories:
✔️ Data Scientists emerged as the highest earners, with an average max salary of $150,000, followed by Data Analysts and Machine Learning Engineers.
✔️ While California, Massachusetts, and Virginia had the highest number of data jobs, it was Delaware that stood out with the highest single maximum average salary around $331,000 
   followed by North Carolina.
✔️ Interestingly, the highest average salaries were reported by mid-sized companies (51–200 employees), closely followed by large enterprises (5001–10,000 employees), a surprising twist 
    that defied some expectations.

