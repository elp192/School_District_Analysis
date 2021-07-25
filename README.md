# School District Analysis
## Project Overview
### Background
The Input Data file consists of [student_complete.csv](https://github.com/elp192/School_District_Analysis/blob/848b49cf0e2d54259f47046b611cac713bee394e/Inputs%20Data/students_complete.csv) and [school_complete.csv](https://github.com/elp192/School_District_Analysis/blob/848b49cf0e2d54259f47046b611cac713bee394e/Inputs%20Data/schools_complete.csv), which include information about 15 schools and 39170 students. The students are at their 9th-12th grade level. In these files, students' math and reading scores and their genders are provided. Analysis of these datasets helps the school board to make an appropriate decision about school budgets and priorities.<br>
### Purpose
The main aim of this project is aggregating data to determine the school performance using math scores, reading scores, and other information that is available about school.<br>
Python (version 3.8.8) is used as the coding language, and the code is written in Jupyter Notebook. Also, Pandas library (version 1.3.0) and Numpy library (version 1.21.0) are utilized in this project.<br>
## Results<br>
ّThe school board finds out dishonesty for the math and reading scores of ninth-graders studied at Thomas High School. To present the standard test scores, these grades should be replaced by NAN values while the rest of the data is kept intact.<br> 
The analysis of the modified database can be categorized as follows:<br>1. District summary, 2. School district summary, 3. Performance of top 5 and bottom 5 schools, 4. The average math and reading scores for 9th-12th graders and each school, 5. The scores that are grouped by: school spending per student, school size, and school type.<br>
### District summary
Among the considered criteria (See Figure 1' headers), it is observed that the dataset modification alters the average math score, passing math and reading percentage, and overall passing percentage related to 15 high schools as follows:<br>
- The average math score is dropped by about 0.1.<br>
- The average reading score is unchanged.<br>
- The percentages of passing math and reading are decreased from 75% to 74.8% and 86% to 85.7%, respectively.<br>
- The percentage of overall passing is dropped from 65% to 64.9%.

:ballot_box_with_check: Overall, modification of dataset causes minor changes in the criteria investigated in this part.<br>

<p img align="center" width="100%">
   <img width="700" alt="Before data modification" src="https://user-images.githubusercontent.com/85843401/126786361-eeecae1c-cff3-4de2-b8d0-030e14672f10.png">
   <img width="700" alt="After data modification" src="https://user-images.githubusercontent.com/85843401/126786580-71c4e17c-627c-4206-a131-5949e2748423.png"><figcaption>Figure 1: Comparison of district summary. Upper: before database modification, Lower: after database modification (i.e., replacing data by NaNs for 9th graders studied at Thomas High School).</figcaption></figure>
</p> 

### School summary
In this section, the information of Thomas High School, affected by alternations of the dataset, is reported (See Figure 2). The observations are as follows:<br>
- The changes in average math and reading scores are negligible, and the scores stayed at the similar values.<br>
- The passing math and reading percentage are decreased significantly by about 28% (from 93.3% to 66.9% and 97.3% to 69.7%, respectively).<br>
- The overall passing percentage is considerably reduced by about 28% (from 90.9% to 65.07%).

:ballot_box_with_check: Overall, the replacement of 9th graders has significant impacts on decreasing passing math, reading, and overall passing percentage.<br>
The information about other schools can be seen in these links: [before database modification](https://github.com/elp192/School_District_Analysis/blob/e056e8e4a3df4e63392aea0169865ed4a0de074c/Results/summary_school_data_before_modification.png), [after database modification](https://github.com/elp192/School_District_Analysis/blob/e056e8e4a3df4e63392aea0169865ed4a0de074c/Results/summary_school_after_data_modification.png).

<p img align="center" width="100%">
  <img width="700" alt="THS_summary_before_modification" src="https://user-images.githubusercontent.com/85843401/126881980-d74da6bb-548e-4657-8cfc-f0e82e0a6f65.png">
  <img width="700" alt="THS_summary_after_modification" src="https://user-images.githubusercontent.com/85843401/126881938-3bc90719-1649-42a0-845a-8a6f8acd2415.png">
<figcaption>Figure 2: Comparison of Thomas High School summary. Upper: before modification of dataset, Lower: after modification of dataset (Replacing data by NaNs for 9th graders at Thomas High School).  </figcaption></figure>
</p> 

### Performance of top 5 and bottom 5 schools
As it is listed below, the school ranking is changed after data modification.<br>
- The overall rating percentage of the Thomas High School is decreased from 91% to 65% (about 28% reduction).<br>
- In the original database, Thomas High School ranked 2nd among all high schools and is considered as the top 5 schools. After modification database, this rank is dropped to 8th place.<br>
- The bottom 5 rank schools remained unchanged.<br>

:exclamation: Hint: The above conclusion is when the number of students who get NAN score (9th graders) are considered in the calculation of total number of students in Thomas High School (See [the performance of schools 1](https://github.com/elp192/School_District_Analysis/blob/e056e8e4a3df4e63392aea0169865ed4a0de074c/Results/performance1_after_data_modification.png)); however, if the 9th-grade students are eliminated from the calculation, the results are changed (See [the performance of schools 2](https://github.com/elp192/School_District_Analysis/blob/e056e8e4a3df4e63392aea0169865ed4a0de074c/Results/performance2_after_data_modification.png)). For example, the Thomas High School rank is still 2, and the overall passing percentage is decreased from 97% to 93%. See this [Figure](https://github.com/elp192/School_District_Analysis/blob/e056e8e4a3df4e63392aea0169865ed4a0de074c/Results/Performance_before_data_modification.png) (related to the dataset before data modification) for comparing the performance of schools before and after dataset modification.

### The average math and reading scores
**School spending per students**<br>
The criteria for school spending range less than $625 and above $645 remained the same (See Figure 3) because the Thomas High School is categorized in the range of $630-644.<br>
 - The passing math and reading percentage is decreased by about 8%.<br>
 - The overall passing percentage is reduced by about 11% (from 63% to 56%).<br>
 - The average math and reading score stayed intact.<br>

<p img align="center" width="100%">
  <img width="500" alt="spending per school_before modification" src="https://user-images.githubusercontent.com/85843401/126882851-f23765f0-45e2-4237-b528-34ea5ade9d18.png">
  <img width="500" alt="spending_school_after_data_modification" src="https://user-images.githubusercontent.com/85843401/126887582-aed89b6b-54d8-4092-8c83-35ba9a9d4ce4.png"><figcaption>Figure 3: Comparing school spending per students. Upper: before database modification, Lower: after database modification (i.e., replacing data by NaNs for 9th graders studied at Thomas High School).</figcaption></figure>
</p>
:exclamation:Hint: Similar to the previous part, the above conclusion is when the number of students who get NAN score (9th graders) is considered in the calculation of the total number of students in Thomas High School; however, if the 9th-grade students are eliminated from the calculation, the conclusion is changed. For example, there is not a significant difference between the results before and after modification of the dataset.

**School size**<br>
The criteria for schools with the size of small and large remained the same (See Figure 3) because the Thomas High school is categorized as the medium school.<br>
- The passing math and passing reading percentage is decreased by about 6% (From 94% to 88% and from 97% to 91%, respectively).<br>
- The overall passing percentage is reduced by about 6.5% (from 91% to 85%).<br>
- The average math and reading score stayed intact.<br>

<p img align="center" width="100%">
   <img width="500" alt="schoolsize_before_data_modification" src="https://user-images.githubusercontent.com/85843401/126888405-45f6a752-0f7f-414e-a1f7-4de72e38b440.png">
   <img width="500" alt="schoolsize_after_data_modification" src="https://user-images.githubusercontent.com/85843401/126888407-6db9e538-465a-42f9-ad3f-a6934881ed8e.png"><figcaption>Figure 3: Comparison of school size. Upper: before database modification, Lower: after database modification (i.e., replacing data by NaNs for 9th graders studied at Thomas High School).</figcaption></figure>
</p> 
:exclamation:Hint: Similar to the previous parts, the above conclusion is when the number of students who get NAN score (9th graders) is considered in the calculation of the total number of students in Thomas High School; however, if the 9th-grade students are eliminated from the calculation, the conclusion is changed. For example, there is not a significant difference between the results before and after modification of the dataset.

**School type**<br>
The criteria for school type known as district remained the same (See Figure 5) because the Thomas High School is categorized as the Charter school.<br>
  - The passing math and passing reading percentage is decreased by about 4% (from 94% to 90% and 97% to 93%, respectively).<br>
  - The overall passing percentage is reduced by about 3% (from 90% to 87%).<br>
  - The average math and reading score stayed unchanged.<br>
 
<p img align="center" width="100%">
   <img width="500" alt="Schooltype_befor_modification" src="https://user-images.githubusercontent.com/85843401/126871926-5e963e49-6d50-4bea-9625-c963f851470a.png">
   <img width="500" alt="schooltype_after" src="https://user-images.githubusercontent.com/85843401/126871929-3cdc5391-f6e5-4b81-848f-e1e33ee3dc53.png"><figcaption>Figure 5: Comparison of school type. Upper: before database modification, Lower: after database modification (i.e., replacing data by NaNs for 9th graders studied at Thomas High School).</figcaption></figure>
</p>
:exclamation:Hint: Similar to the previous parts, the above conclusion is when the number of students who get NAN score (9th graders) is considered in the calculation of the total number of students in Thomas High School; however, if the 9th-grade students are eliminated from the calculation, the conclusion is changed. For example, there is not a significant difference between the results before and after modification of the dataset.

## Summary
 The results of dataset before and after replacing the 9th grader scores for the Thomas High School by NAN are compared. Following essential changes are observed in our analysis:<br>
- The summary school results represent the significant score reduction for the overall passing percentage of Thomas high school. Also, the related passing maths and reading percentage are dropped.<br>
- The ranked place of Thomas high school is dropped from 2nd to 8th.<br>
- The math and reading scores for 9th graders studied at Thomas High School are not available for analysis. Also, if the number of 9th graders is eliminated from the total number of students at this school, the conclusion is different in comparison to the case that the number of students with NAN values is considered in the analysis <br>
- Analysis of average math and reading scores grouped by school spending per student, school size, and school type represents the reduction of passing math and reading, and overall percentage for those that are classified in spending school range $630-644, medium sizes of school, and Charter schools.<br>
