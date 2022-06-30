# School_District_Analysis

## Overview
In this project, I analyzed data on student funding and students' standardized test scores. I got two CSV files, school_complete.csv and students_complete.csv, that hold all the schools' information in the district and student academic performance in reading and math. 

Within the module, I explored the datasets, checked for missing values, merged DataFrames,  and gave a summary of all the schools' budget information and students' academic performance in reading and math. Then, I analyzed the school's performance based on the budget per student, the school size, and the type of school. After I finished the above analysis with Python in Jupyther Notebook, I was notified by the school board that there is evidence of academic dishonesty in reading and math grades for Thomas High School ninth graders. Their grades might be altered. Under this circumstance, I replaced the math and reading scores for Thomas High School ninth graders with NaNs in the dataset. Then I redid the whole analysis and compared the initial results with the modified ones to check if these changes affected the overall analysis.  

### Purpose
The purpose of this project is to utilize the Python Pandas library to aggregate the data and showcase trends in school performance. This analysis will assist the school board in making decisions about the school budget allocation and funding priorities.
    
## Analysis Results   
### District Summary
In the initial district summary, the total budget for all the 15 schools in the district is $24.6 million. Average math score is 79. Average reading score is 81.9. The passing score is 70 for both math and reading tests. 75% of the students in the school district passed math. 85.8% of students passed reading. However, the overall passing percentage that both passed math and reading tests is only 65.2%. 
 With Thomas High School 9th graders's records replaced with NaNs in the DataFrame and 9th graders removed from total student count, the average score for math and math passing rate turned a little lower than the ones shown in the initial summary table. The average reading socre kept the same in the new district summary table. The reading passing rate and the overall passing rate all turned lower than the original numbers. The district summary was not affected that much.
 the average score for math and reading are a little lower than the ones shown in the initial summary table. The same for the math, reading, and overall passing rates.  
![District Summary Original](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/District%20Summary%20Original.png)

![District Summary with Thomas High 9th graders' records removed](https://github.com/Wuyang080510/School_District_Analysis/blob/main/School%20District%20Analysis%20Images/District%20Summary%20(with%20THS%209th%20grade%20student%20removed).png)

    Results: Using bulleted lists and images of DataFrames as support, address the following questions.
        How is the district summary affected?
        How is the school summary affected?
        How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
        How does replacing the ninth-grade scores affect the following:
            Math and reading scores by grade
            Scores by school spending
            Scores by school size
            Scores by school type

    Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.




     
    
    
     
