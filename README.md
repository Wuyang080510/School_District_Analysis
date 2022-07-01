# School_District_Analysis

## Overview
In this project, I analyzed data on student funding and students' standardized test scores. I got two CSV files, school_complete.csv and students_complete.csv, that hold all the schools' information in the district and student academic performance in reading and math. 

Within the module, I explored the datasets, checked for missing values, merged DataFrames,  and gave a summary of all the schools' budget information and students' academic performance in reading and math. Then, I analyzed the school's performance based on the budget per student, the school size, and the type of school. After I finished the above analysis with Python in Jupyther Notebook, I was notified by the school board that there is evidence of academic dishonesty in reading and math grades for Thomas High School ninth graders. Their grades might be altered. Under this circumstance, I replaced the math and reading scores for Thomas High School ninth graders with NaNs in the dataset. Then I redid the whole analysis and compared the initial results with the modified ones to check if these changes affected the overall analysis.  

### Purpose
The purpose of this project is to utilize the Python Pandas library to aggregate the data and showcase trends in school performance. This analysis will assist the school board in making decisions about the school budget allocation and funding priorities.
    
## Analysis Results   
### District Summary
- In the initial district summary, the total budget for all the 15 schools in the district in 2019 was $24.6 million. The average math score was 79. The average reading score was 81.9, about 2 points higher than the average math score. The passing score was 70 for both math and reading tests. 75% of the students in the school district passed math. 85.8% of students passed reading. However, the overall passing percentage of students who passed math and reading tests was only 65.2%. 

![District Summary Original](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/District%20Summary%20Original.png)
Table-1 District Summary(initial version)

- With Thomas High School 9th graders' records replaced with NaNs in the DataFrame and 9th graders removed from the total student count, the average math and math passing rate score turned slightly lower than the ones shown in the initial summary table. The average reading score kept the same in the new district summary table. The reading passing rate and the overall passing rate all turned lower than the original numbers. With the change, the district summary was not affected that much. 

![District Summary with Thomas High 9th graders' Records Altered](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/District%20Summary%20(with%20THS%209th%20grade%20student%20removed).png)
Table-2 District Summary with Thomas High School 9th Graders's Records Removed from the Total Count

### School Summary
- According to the original dataset, the school district had eight charter schools and seven public schools in 2019.
- The fund allocated to each student ranged from $578 to $655. Wilson High School had the lowest amount of funds allocated to each student. Huang High School has the highest per-student budget. 
- The average math score ranged from 76.6 to 83.8, with the passing percentage ranging from 65.7% to 94.6%. Huang High School had the lowest math passing rate, while Pena High School had the highest math passing rate. 
- The average reading score ranged from 80.7 to 84.0, with the passing percentage ranging from 79.3% to 97.1%. Ford High School had the lowest reading passing rate, while Griffin High School had the highest reading passing rate. 
- The overall passing percentage had a lower bound of 53.0%, which is Rodriguez High School. Cabrera High School had the highest overall passing rate of 91.3%. The overall passing percentage is lower than the individual subject passing rate. 

![Per School Summary](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/Per%20School%20Summary-original.png)
Table-3 School Summary(initial version)

- With Thomas High School 9th graders' records replaced with NaNs in the DataFrame and 9th graders removed from total student count,
the performance scores for Thomas High School had a slight dip, as shown in the table below.

![Per School Summary with Thomas High School 9th Graders' Records Altered](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/per%20school%20summary%20with%20scores%20and%20passing%20percentage%20of%20THS%20replaced.png)
Table-4 School Summary with Thomas High School 9th Graders's Records Removed from the Total Count

- Replacing the ninth graders’ math and reading scores had no significant affection on Thomas High School’s performance relative to the other schools. Thomas High School kept outperforming the other schools in the school district. 

### Math and Reading Scores by Grade
- There is not much difference in the average math and reading scores in different grades. 
- As the ninth graders' math and reading scores of Thomas High School were replaced with NaNs, the summary table shows NaN in the 9th Grade Avg Math Score column and the 9th Grade Avg Reading Score column.

![Math Scores by Grade](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/per%20school%20math%20score%20by%20grades.png)
Table-5 Math Scores by Grade
![Reading Scores by Grade](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/per%20school%20reading%20score%20by%20grades.png)
Table-6 Reading Scores by Grade

### Scores by School Spending
- Interestingly, the more funds schools spent on each student, the lower the scores were. The same applies to the passing percentage of math, reading, and both subjects. 
- The school district board should conduct further investigations to find the reasons for this result. Is it because schools spent most of the funds on upgrading infrastructure rather than hiring experienced teachers? Or is the academic education program school purchased not fit students' needs?
- As the score changes of Thomas High School did not significantly affect Thomas High School's academic performance, the change did not affect the Scores by School Spending analysis that much. The percentage of passing reading for schools in the spending range of $631-645 turned 0.1% lower after the score changes. The overall passing rate for the schools in the same spending range had a dip of 0.1%.

![Scores by School Spending](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/scores%20by%20school%20spending.png)
Table-7 Scores by School Spending

### Scores by School Size
- From the table, smaller schools tend to have better academic performance. Schools with 2000 to 5000 students had the lowest overall passing percentage of 58.3%.
- As the score changes of Thomas High School did not significantly affect Thomas High School's academic performance, the change did not affect the Scores by School Size analysis a lot. Only the reading passing rate for medium-sized schools turned 0.1% lower after the score changes.  

![Scores by School Size](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/scores%20by%20school%20size.png)
Table-8 Scores by School Size

### Scores by School Type
- From the table, charter school students achieved better academic performance in 2019. Math is the shortboard for district schools. The percentage of students who passed the math tests for district schools was 29% lower than the charter schools. The average math score of district schools is 77.0, 6.5 points lower than charter schools in the same school district. The percentage of students who passed the reading tests in district schools was 15.8% lower than the pass rate at charter schools. 90.4% of charter school students passed both math and reading test in 2019. The overall passing rate for district schools is only 53.7%. District schools need to do more to improve students' academic performance. 
- The score changes of Thomas High School slightly affected the academic performance of Thomas High School. With the numbers averaged, the change did not affect the Scores by School Size analysis. 

![Scores by School Type](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/scores%20by%20school%20type.png)
Table-9 Scores by School Type        
    
## Summary
With Thomas High School 9th graders' scores were replaced with NaNs:
- The average score for math and math passing rate turned a little lower than the ones shown in the initial district summary table. After the score changes, the reading passing percentage and overall passing percentage were lower than the original numbers in the district summary table.
- The performance scores for Thomas High School dipped slightly in the school summary table. 
- The academic performance summary by grade tables shows "NaN" in the "9th Grade Avg Math Score" column and "9th Grade Avg Reading Score" column for Thomas High School.
- In the "Scores by School Spending" table, the percentage of passing reading for schools in the spending range of $631-645 turned 0.1% lower after the score changes. The overall passing rate for the schools in the same spending range had a dip of 0.1%.
- In the "Scores by School Size" Table, the reading passing rate for medium-sized schools turned 0.1% lower after the score changes.  
