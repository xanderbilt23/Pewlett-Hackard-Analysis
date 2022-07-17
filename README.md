# Pewlett-Hackard-Analysis

## Overview

Determined the number of retiring employees per title, and identified employees who are eligible to participate in a mentorship program as many current employees at Pewlett Hackard are reaching retirement age.

## Results

- Largest number of employees that are eligible to retire are Senior Engineers or Senior Staff.
- There are 1,549 employees that are eligible for the mentorship program.
- There are a total of 72,458 employees that are close to retirement.
- Only 2 employees that are a in a manager position will retire in the forseeable future.

![retiring_titles_table](https://github.com/xanderbilt23/Pewlett-Hackard-Analysis/blob/main/Resources/retiring_titles_table.png)

## Summary

### How many roles will need to be filled as the "silver tsunami" begins to make an impact?

- A total of 72,458 roles will need to be filled.

```
-- Query ran to retrieve the sum of the count titles in retiring_titles table

SELECT SUM (count)
FROM retiring_titles;
```

### Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewelett Hackard employees?

- There are not enough qualified retirement-ready employees in the departments to mentor the next generation of Pewelett Hackard as there are only 1,549 retirement ready employees to mentor 72,458 positions.

```
-- Query ran to retrieve count of mentor eligible employees in the mentorship_eligibilty table

SELECT COUNT (emp_no)
FROM mentorship_eligibilty;
```
