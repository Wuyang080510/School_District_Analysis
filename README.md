# School_District_Analysis

## Overview
In this project, I analyzed data on student funding and students' standardized test scores. I got two CSV files, school_complete.csv and students_complete.csv, that hold all the schools' information in the district and student academic performance in reading and math. 

Within the module, I explored the datasets, checked for missing values, merged DataFrames,  and gave a summary of all the schools' budget information and students' academic performance in reading and math. Then, I analyzed the school's performance based on the budget per student, the school size, and the type of school. After I finished the above analysis with Python in Jupyther Notebook, I was notified by the school board that there is evidence of academic dishonesty in reading and math grades for Thomas High School ninth graders. Their grades might be altered. Under this circumstance, I replaced the math and reading scores for Thomas High School ninth graders with NaNs in the dataset. Then I redid the whole analysis and compared the initial results with the modified ones to check if these changes affected the overall analysis.  

### Purpose
The purpose of this project is to utilize the Python Pandas library to aggregate the data and showcase trends in school performance. This analysis will assist the school board in making decisions about the school budget allocation and funding priorities.
    
## Analysis Results   
### District Summary
- In the initial district summary, the total budget for all the 15 schools in the district is $24.6 million. Average math score is 79. Average reading score is 81.9, about 2 points higher than the average math score. The passing score is 70 for both math and reading tests. 75% of the students in the school district passed math. 85.8% of students passed reading. However, the overall passing percentage that both passed math and reading tests is only 65.2%. 

![District Summary Original](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/District%20Summary%20Original.png)
Table-1 District Summary

- With Thomas High School 9th graders's records replaced with NaNs in the DataFrame and 9th graders removed from total student count, the average score for math and math passing rate turned a little lower than the ones shown in the initial summary table. The average reading socre kept the same in the new district summary table. The reading passing rate and the overall passing rate all turned lower than the original numbers. With the change, the district summary was not affected that much. 
 

![District Summary with Thomas High 9th graders' Records Altered](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/District%20Summary%20(with%20THS%209th%20grade%20student%20removed).png)
Table-2 District Summary with Thomas High School 9th Graders's Records Removed from the Total Count

### School Summary
- Based on the original data, there are 8 charter schools and 7 public schools in the district.
- The fund allocated to each student ranged from $578 to $655. Wilson High School has the lowest fund allocated to each student. Huang High School has the highest per student budget. 
- The avearge math socre ranged from 76.6 to 83.8 with the passing percentage in the range of 65.7% to 94.6%. Huang High School has the lowest math passing rate, whereas, Pena High School has the highest math passing rate. 
- The average reading socre ranged from 80.7 to 84.0 with the passing percentage in the range of 79.3% to 97.1%. Ford High School has the lowest reading passing rate, whereas, Griffin High School has the highest reading passing rate. 
- The overall passing percentage has a lower bound of 53.0%, which is Rodriguez High School. Cabrera High School has the highest overall passing rate of 91.3%. The overall passing percentage is lower than the individual subject passing rate. 

![Per School Summary](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/original%20per%20school%20summary.png)
Table-3 School Summary

- With Thomas High School 9th graders's records replaced with NaNs in the DataFrame and 9th graders removed from total student count,
the performance scores for Thomas High School has a slight dip as shown in the following table.

![Per School Summary with Thomas High School 9th Graders' Records Altered](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/per%20school%20summary%20with%20scores%20and%20passing%20percentage%20of%20THS%20replaced.png)
Table-4 School Summary with Thomas High School 9th Graders's Records Removed from the Total Count

- Replacing the ninth graders’ math and reading scores had no significant affection on Thomas High School’s performance relative to the other schools. Thomas High School kept outperforming the other schools in the school district. 

### Math and Reading Scores by Grade
- There is not much difference in the average math and reading scores in different grades. 
- As the ninth graders' math and reading scores of Thomas High School were replaced with NaNs, the summary table shows nan in the "9th Grade Avg Math Score" column and "9th Grade Avg Reading Score" column.

![Math Scores by Grade](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/per%20school%20math%20score%20by%20grades.png)
Table-5 Math Scores by Grade
![Reading Scores by Grade](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/per%20school%20reading%20score%20by%20grades.png)
Table-6 Reading Scores by Grade

### Scores by School Spending
- It is very interesting to see that the more fund schools spent in each student, the lower the scores were. The same thing applies to the passing percentage of math, reading, and both subjects. 
- The school district board should make further investigation to find the reasons lead to this result. Is it because schools spent most of the fund on upgrading infrastructure rather than hiring experienced teachers? Or is the academic education program school purchased did not fit students' needs?
- As the score changes of Thomas High School did not had a significant effect in Thomas High School's academic performance, the change did not affect the Scores by School Spending analysis.

![Scores by School Spending](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/scores%20by%20school%20spending.png)

### Scores by School Size
- From the table, smaller schools tend to have better academic performance. Schools with 2000 to 5000 students had the lowest overall passing percentage of 58.3%
- As the score changes of Thomas High School did not had a significant effect in Thomas High School's academic performance, the change did not affect the Scores by School Size analysis.

![Scores by School Size](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/scores%20by%20school%20size.png)

### Scores by School Type
- From the table, charter school students achieved better academic performance in 2019. Math is the shortboard for district schools. The average math score for district schools were 29 points lower than the charter schools. 

![Scores by School Type](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/scores%20by%20school%20type.png)
        
    

    Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.




     
    
    
     
