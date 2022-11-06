# Pewlett-Hackard-Analysis
This project consists in creating ERD (Entity Relationship Diagrams) to develop data queries and modeling, to further perform a complete analysis on Pewlett-Hackard information using SQL practices.


## Overview of the analysis
Pewlett Hackard a large company is looking toward several employee-retirements, so they are preparing for the future in two ways. Therefore, they need to find answers to the following questions: Who will be retiring in the next few years? And how many positions will Pewlett Hackard need to fill? So, considering that the information they have is only available in the form of CSV files (6 different files), this analysis will help Pewlett Hackard determine the number of retiring employees per title that are elegible for the retirement package. Likewise, it will also assist to identify employees who are eligible to participate in a mentorship program. 

## Results
The first step of the analysis consisted in developing an ERD to understand the relationship that exist between the different CSV files provided. After that it was necessary to create a Retirement Titles table that holds all the titles of employees considering certain criteria (employees that were born between January 1, 1952 and December 31, 1955) that show who are the employees that are close to be retired.

As a preliminary result, we encountered that there were duplicate entries for certain employees whose show multiple titles (it may be due to promotions). This is illustrated in the following table - Retirement_titles Table

![Image](https://github.com/rdonosob1/Pewlett-Hackard-Analysis/blob/main/retirement_titles%20TABLE.png)

Due to that, it was essential to perform a new query to obtain a cleaner data. Therefore, the following table illustrates the data with the most recent titles per employee, as well as filtering employees that had left the company.  information Unique _titles Table

![Image](https://github.com/rdonosob1/Pewlett-Hackard-Analysis/blob/main/unique_titles%20TABLE.png)

Consequently, an additional query needed to be written to count and retrieve the number of employees by their most recent job title who are about to retire per department. Retiring_titles Table.

![Image](https://github.com/rdonosob1/Pewlett-Hackard-Analysis/blob/main/retiring_titles%20TABLE.png)

Finally, as mentioned above Pewlett Hackard was also looking to identify employees who are eligible to participate in a mentorship program. Therefore, the Second part of this analysis consisted in writing a query to create a table (Mentorship_Eligibility table) that shows the employees who are eligible to participate in a mentorship program. 

![Image](https://github.com/rdonosob1/Pewlett-Hackard-Analysis/blob/main/mentorship_eligibilty%20TABLE.png)

## Summary
As a result of this analysis, the count list above indicates that around 72,400 employees will retire in the next few years. Most of them holding senior positions (around 50,000 employees).  

Finally, the second part of the analysis shows that there are over 1500 employees that were born between 1965-01-01 and 1965-12-31, and therefore are eligible to participate in a mentorship program.

  o	How many roles will need to be filled as the "silver tsunami" begins to make an impact?
 
 	• There are over 70,000 jobs that will be vacant due to the "silver tsunami" and there will need to be filled. This represents around 24% of the total vacants of the  company since it has around 300,000 employees. 
  
  o Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

  •	Based on that, the answer to this question is yes. There are enough qualified retirement-ready employees to mentor the next generation since they represent almost 1/4 of PH workfore. 
