# School_District_Analysis

## Overview of Project

**Purpose:**  
Maria works for the city school systems, she has asked us for help with performing an analysis on standardized test scores for math and reading to see if there is a relationship with school spending, school size, and school type. This would help the school board make decisions on school budgeting and priorities. The purpose of this project is to perform an analysis to discover if there is any trends with school factors and school performance on standardized tests based on individual schools and at the district level.  

## Resources:
- Data Source: schools_complete.csv, students_complete.csv, clean_students_complete.csv
- Software: Python 3.9.7, Anaconda 4.10.3, Jupyter Notebook 6.4.5

## Analysis and Results

**Analysis:**  
For this analysis, we were provided with a dataset for student data and a dataset for school data. The student information had information on student name and ID, where the students went to school, both their math and reading grades, and their grade level in school. The school dataset has information on the school name, the type of school (district or charter), number of students, and spending budget. With this information from our dataset, we are able to calculate number of students that passed math and reading, as well as passing both math and reading. A score of 70 or greater would be considered passing for this analysis. Once we have the number of students that are passing for each of those three categories, we can calculate the percent of students passing by dividing by the total number of students in the district. Maria was also wanting us to analyze to see if there is a the relationship of test scores by school spending, by school size, and by school type. This would give her, as well as the school board, a better understanding if there is any impact on the students' test scores based on those individual factors.  

After performing the initial analysis, we were informed that test scores for 9th graders at Thomas High School were compromised. This means that we would have to perform another analysis without those test scores included in our dataset as it may change our end results. Fortunately for us, we can use this new found data and compare it to the first analysis that we performed to give a deeper understanding on how this impacts our overall results if in case something like this happens again in the future.  



**Results:**  
- How is the district summary affected?  
We can see that there is very minimal change across the board for average passing scores, passing percentage, and overall passing percentage. Per attached images, with the first image being from our inital analysis and the second image being from our recalculated results.  
<img src="Resources/Initial_district_summary_picture.PNG">  
<img src="Resources/Second_district_summary_picture.PNG">  

- How is the school summary affected?  
After we removed the test scores from the 9th graders at Thomas High School, we performed the same calculations with the upperclass (10th through 12th graders). From our results, we noticed very minimal change in our data. We found that there was about a change of 0.05 point change in average scores for both math and reading, which is about 0.1% to 0.3% change in percent passing for math and reading respectively and an overall percent passing change of 0.3%. Attached are 2 images of the top 5 schools in the district with the first image from our initial analysis, and the latter from our second analysis. Since Thomas High School was the only school that had compromised data, we mainly need to look at that particular school to see if there is any change in results.  
<img src="Resources/Initial_top_five_schools.PNG">  
<img src="Resources/Second_top_five_schools.PNG">  

- How does replacing the 9th graders' math and reading scores affect Thomas High School's performance relative to the other schools?  
As noted in the school summary and the images above, there was minimal change in math and reading test scores, therefore there was no significant change in school performance relative to the other schools.  

- How does replacing the 9th graders' scores affect math and reading scores by grade?  
Obviously, we replaced 9th grade test scores with "NaN" and we did not change anything with the upperclass test scores. Therefore the upperclass test scores had no change. But there was minimal change for ninth graders in all the schools in the district, with a change of -0.1% for reading and -0.2% for math. The first image is from our initial analysis, and the second image is from our second analysis.  
<img src="Resources/Initial_average_ninth_scores.PNG">  
<img src="Resources/Second_average_ninth_scores.PNG">  

- How does replacing the 9th graders' scores affect scores by school spending?  
Scores by school spending was not affected when replacing 9th graders' scores with "NaN".  
<img src="Resources/Combined_scores_by_school_spending.PNG">  

- How does replacing the 9th graders' scores affect scores by school size?  
Scores by school size was not affected when replacing 9th graders' scores with "NaN".  
<img src="Resources/Combined_scores_by_school_size.PNG">  

- How does replacing the 9th graders' scores affect scores by school type?  
Scores by school type was not affected when replacing 9th graders' scores with "NaN".  
<img src="Resources/Combined_scores_by_school_types.PNG">  


## Challenge Summary

**Summary**  
For this analysis, we did a comparision of math, reading and both combined math and reading scores for 15 schools in a single school district. We compared school spending, school size, and school type with the standardized test score results to see if there is any relationships or treads on student performance. For our analysis, we found minimal to no change (no significant changes) in our results. Part of why there may have been minimal to no change in our analysis because the school district has 39,170 students and only 461 students in the 9th grade at Thomas High School which makes up ~1% of the population in our analysis. Therefore, any change in that population would have a low impact on the overall data that we are studying. Another reason why there might be minimal to no change could be related to the test scores of 9th graders that were taken out. We calculated the average and percent passing for both math and reading, the average test scores of the 9th graders at Thomas High School was 83.6 for math and 83.7 for reading. These scores are very close to the overall average of 78.9 for math and 81.9 for reading for all of the 9th graders, which is why there wouldn't be any dramatic changes after the test scores were removed. In conclusion, removing a small population with a close to the overall average test scores would have minimal impact on the overall results.  

### Codes Used  
<img src="Resources/Code1.PNG">  
<img src="Resources/Code2.PNG">  
<img src="Resources/Code3.PNG">  
<img src="Resources/Code4.PNG">  
<img src="Resources/Code5.PNG">  
<img src="Resources/Code6.PNG">  
<img src="Resources/Code7.PNG">  
<img src="Resources/Code8.PNG">  
<img src="Resources/Code9.PNG">  
<img src="Resources/Code10.PNG">  
<img src="Resources/Code11.PNG">  