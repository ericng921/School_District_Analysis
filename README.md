# School_District_Analysis

## Overview of the school district analysis
### Purpose of the analysis

In the previous module practice, we had done a comprehensive school district analysis based on the two datasets - schools_complete and students_complete. However, the school board had noticed that the math and reading grades for Thomas High School (THS) ninth grades appear to have been altered. The purpose of the analysis is that we need to replace the 9th reading and math scores with NaN and to obtain updated results.

After replacing the ninth-grades scores we calculated the new student count for all the school without 9th grade student. Based on the new student account we got the passing percentages for math and reading, overall passing percentage, new district summary, new school summary with updated Thomas High School 10th to 12th grades only. 

In addition, we obtained the top 5 and bottom 5 overall passing results, new math and reading score in new dataframe for each grade from each school using groupby function, scores by school spending per student, by school size, and by school type through spending bins method for a deeper analysis.

## Results:

- How is the district summary affected?
    The district summary has a minor impact because there are only 461 THS 9th grade student excluded compare to a total of 39170 students in 15 schools.

- How is the school summary affected?
    Thomas High School is moved to 2nd with highest overall passing percentage from 8th of 15 schools.

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
    The overall performance is much better after replacing the THS 9th grade math and reading scores. It became 2nd of 15 schools with highest overall passing percentage and also moved from bottom to 2nd for Charter School Type schools.

- How does replacing the ninth-grade scores affect the following:

    * Math and reading scores by grade
    
    Math and reading scores by grade are showing NaN for Thomas High School 9th grade 
    Math 

    * Scores by school spending

    The spending ranges for THS is changed to $630-644. However, there is a very minor impact for the data

    * Scores by school size
    THS is medium size (1000-2000) and the scores by school size has a very minor impact as picture shown below

    * Scores by school type
    THS is a Charter School Type. The scores by school type have a very minor impact as well as picture shown below.

## Summary

There are Four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School (THS) have been replaced with Nans:

1. Student dataset and Scores by Grade dataframe will show NaN on Reading and Math Scores for THS 9th grade student.

2. For THS % of overall passing, it is increased from 65.08% to 90.63% after omitting the ninth-grade students.

3. The numbers of District summary has been slightly changed. The Average Math Score is -0.05, Average Reading Score is 0.02, % Passing Math is -0.22, the % Passing Reading is -0.15, and % Overall Passing is -0.32. These changes are minor because there are only 461 ninth grade student from THS excluded, it is not a big number compare to total students of 39170.

4. THS became 2nd of top 5 school with highest overall passing percentage also 2nd of top Charter school type schools, compare to 8th of 15 school and bottom of Charter school type school before replacing with Nans.



