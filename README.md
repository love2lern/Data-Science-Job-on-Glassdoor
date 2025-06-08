# Data-Science-Job-on-Glassdoor

Project Name
"Data Science Job Posting on Glassdoor"

Overview
This project analyzes job postings for data science roles listed on Glassdoor. The dataset was sourced from Kaggle under the title "Data Science Job Posting on Glassdoor". The primary goal was to clean, explore, and visualize insights about the job market, including salaries, locations, company types, and required skills.

Dataset
Source: Kaggle
File: CSV format with job listing data scraped from Glassdoor
Main Columns:
o	Company Name
o	Location
o	Salary Estimate
o	Job Description
o	Rating, Founded, Type of ownership, etc.

Data Cleaning
•	Removed rows with -1 or null values in important columns (Industry, Sector, Headquarters, Founded)
•	Dropped irrelevant or duplicate columns (e.g., index, Competitors)
•	Converted salary fields to numeric values after extracting numbers from text
•	Reset DataFrame index and dropped duplicates

Feature Engineering
•	Location Split: Split Location into City and State
•	Salary Columns: Extracted MinSalary, MaxSalary, and calculated Salary Average
•	Skills: Created binary columns for the presence of keywords like python, excel, aws, spark, etc. in Job Description
•	Ownership Type: Normalized values in Type of ownership column

Data Analysis & Visualization
•	Top Hiring Cities: Pie chart showing job distribution by city
•	Skill Demand: Bar plots showing frequency of skill mentions
•	Salary Distribution: Histogram of average salary
•	Correlation Heatmap: Showed relationships between key numeric variables
•	Top Companies by Salary: Sorted companies based on Salary Average

Key Insights
•	Python and Excel were the most in-demand skills
•	Public companies dominated the job listings
•	California and New York were the top hiring states
•	Higher ratings and older companies tended to offer better salaries

Tools & Libraries
•	Python (Jupyter Notebook)
•	pandas
•	matplotlib
•	seaborn

How to Run
1.	Clone the repo
2.	Install requirements: pip install -r requirements.txt
3.	Open DS Job cleaning.ipynb in Jupyter Notebook
4.	Run cells in order to reproduce analysis

Conclusion
This project provides a complete EDA of Glassdoor job postings for data science roles. It shows how data can be cleaned, transformed, and analyzed to extract valuable job market insights.

Project by [Fatemeh Saderi]

