# School_District_Analysis

## Overview of the school district analysis
### Purpose of the analysis

In the previous module practice, we had done a comprehensive school district analysis based on the two datasets - schools_complete and students_complete. However, the school board had noticed that the math and reading grades for Thomas High School (THS) ninth grades appear to have been altered. The purpose of the analysis is that we need to replace the 9th reading and math scores with NaN and to obtain updated results.

After replacing the ninth-grades scores we calculated the new student count for all the school without 9th grade student. Based on the new student account we got the passing percentages for math and reading, overall passing percentage, new district summary, new school summary with updated Thomas High School 10th to 12th grades only. 

In addition, we obtained the top 5 and bottom 5 overall passing results, new math and reading score in new dataframe for each grade from each school using groupby function, scores by school spending per student, by school size, and by school type through spending bins method for a deeper analysis.

## Results:

- How is the district summary affected?

  The district summary has a minor impact because there are only 461 THS 9th grade student excluded compare to a total of 39170 students in 15 schools.
    
  Original
  ![district_summary](https://user-images.githubusercontent.com/100378319/160249541-c9619996-95b5-469d-a406-004df2d36857.png)
  Updated
  ![update_district_summary](https://user-images.githubusercontent.com/100378319/160249548-167b3d6c-db82-45a2-91c7-a3d6c6d8b47a.png)
  
- How is the school summary affected?
   
  The avgerage Math and reading score are slightly changed, but the overall passing percentage is increased from 65% to 91%. 

Original
<img width="753" alt="original_THS" src="https://user-images.githubusercontent.com/100378319/160249776-55ffbcb7-8c14-4497-9d76-037083970309.png">
Updated
![update_THS](https://user-images.githubusercontent.com/100378319/160249942-feb30dca-c703-48c9-a8fa-cccae8b18adb.png)

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
   
  The overall performance is much better after replacing the THS 9th grade math and reading scores. It became 2nd of 15 schools with highest overall passing percentage and also moved from bottom to 2nd for Charter School Type schools.

Original
![Original_top_school](https://user-images.githubusercontent.com/100378319/160250093-0f82f67b-5efb-4718-8c28-8d33771954ff.png)

Updated
![updated_top_school](https://user-images.githubusercontent.com/100378319/160250097-364dc9e5-fe7c-4efb-b5bf-e294eae01437.png)

- How does replacing the ninth-grade scores affect the following:

    * Math and reading scores by grade    

    Math and reading scores by grade are showing NaN for Thomas High School 9th grade 
    

![new_math_scoresbygrade](https://user-images.githubusercontent.com/100378319/160249597-8d85eda1-9a7c-434b-8623-8db4c9b3bda3.png)

![new_reading_scoresbygrade](https://user-images.githubusercontent.com/100378319/160249601-0398f696-51c5-449b-b24e-f9998363eac8.png)

    * Scores by school spending
   
    The spending ranges for THS is changed to $630-644. However, there is a very minor impact for the data
    
Original
<img width="618" alt="original_per_student" src="https://user-images.githubusercontent.com/100378319/160249642-ce8a6474-be61-4fec-ae52-84a12efc0117.png">

Updated
![updated_per_student](https://user-images.githubusercontent.com/100378319/160249624-3c3207c6-a1bd-438b-974e-f885761aaec4.png)

    * Scores by school size
   
    THS is medium size (1000-2000) and the scores by school size has a very minor impact as picture shown below
    
Original
<img width="563" alt="original_by_school_size" src="https://user-images.githubusercontent.com/100378319/160249693-dee8e194-b50a-4fba-adaf-5616f34b9543.png">

Updated
![update_by_school_size](https://user-images.githubusercontent.com/100378319/160249680-2b8c1683-d02a-4c82-9bdc-c95130ebe53f.png)

    * Scores by school type
    
    THS is a Charter School Type. The scores by school type have a very minor impact as well as picture shown below.
    
Original    
<img width="531" alt="original_by_school_type" src="https://user-images.githubusercontent.com/100378319/160249705-9d1130d1-af02-467b-8715-b1d23a902aa0.png">

Updated
![updated_by_school_type](https://user-images.githubusercontent.com/100378319/160249711-a2ccca53-7d23-43b6-8374-aed0bc5a5b91.png)

    
## Summary

There are Four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School (THS) have been replaced with Nans:

1. Student dataset and Scores by Grade dataframe will show NaN on Reading and Math Scores for THS 9th grade student.

2. For THS % of overall passing, it is increased from 65.08% to 90.63% after omitting the ninth-grade students.

3. The numbers of District summary has been slightly changed. The Average Math Score is -0.05, Average Reading Score is 0.02, % Passing Math is -0.22, the % Passing Reading is -0.15, and % Overall Passing is -0.32. These changes are minor because there are only 461 ninth grade student from THS excluded, it is not a big number compare to total students of 39170.

4. THS became 2nd of top 5 school with highest overall passing percentage also 2nd of top Charter school type schools, compare to 8th of 15 school and bottom of Charter school type school before replacing with Nans.



