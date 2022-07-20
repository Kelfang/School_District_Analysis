# School Data Analysis Project

## Project Overview
  The purpose of this project is to deliver key metrics to assess several schools within a district. Areas of interest include student scores, budgets, school size, and school type. Within the data analyzed, there were over 39,000 students across 15 schools.
  
  After starting my analysis of the data, I was informed that the 9th grade math and reading scores from Thomas High School (THS) were being removed and replaced with a non-numeric variable. This was done to preserve the integrity of the remaining data since replacing the scores with “0” would artificially skewed the district and school performance. 

### Deliverables
  *	A high-level snapshot of district’s key metrics.
  *	An overview of the key metrics for each school within the district.
  *	Tables presenting each of the following metrics:
    -	Top 5 and bottom 5 performing schools
    -	The average math score received by students in each grade at each school
    -	The average reading score received by students in each grade at each school
    -	School performance based on the budget per student
    -	School performance based on the school size
    -	School performance based on the type of school

## Resources 
  *	Software: Python with pandas library
  *	Platforms: Jupyter Notebook, via Anaconda
  *	Data Sources: schools_complete.csv, students_complete.csv

## Summary of Results
  With the omission of the math and reading scores for all the 9th graders at Thomas High School, you will see that the numbers did not vary significantly between the original data and the adjusted data. I will evaluate those variances below.
  
  To give the data more context, a passing score is equal to or greater than 70 in either reading or math. Any references made to “Overall Passing” is defined as a student scoring equal to or greater than 70 in both math and reading. Additionally, all analysis that is shown prior to the removal of the 9th grade THS math and reading scores will be referenced as “Original”. All analysis completed after the removal of the 9th grade THS scores will be referenced as “Adjusted”.

### District Summary
  In reviewing the high-level data, at a district level, you can see that the variances before and after the removal of the 9th grade THS scores is minimal. The greatest change is on the “% Overall Passing” which went down 0.3%, with the second largest change found within the “% Passing Math” at 0.2%. 

*<sub>District Summary Original</sub>*

![ District Summary_Original.png](https://github.com/Kelfang/School_District_Analysis/blob/main/Uploaded%20PNGs/District%20Summary_Original.png)

*<sub>District Summary Adjusted</sub>*

![ District Summary_Adjusted.png](https://github.com/Kelfang/School_District_Analysis/blob/main/Uploaded%20PNGs/District%20Summary_Adjusted.png)


### School Summary
  Drilling down into the data within Thomas High School, you will see that greatest change is reflected in the “% Overall Passing”, just as we did in the district level data, at 0.3%. The reading and math mirrored the district differences as well.
  
  Please take note that the total number of students at THS remain unchanged. The only data points that were omitted were the reading and math scores. This was done to accurately reflect the school size and the budget data that pertains to the student count.

*<sub>Per School Summary Original</sub>*

![Per School Summary_Original.png](https://github.com/Kelfang/School_District_Analysis/blob/main/Uploaded%20PNGs/Per%20School%20Summary_Original.png)

*<sub>Per School Summary Adjusted</sub>*

![ Per School Summary_Adjusted.png](https://github.com/Kelfang/School_District_Analysis/blob/main/Uploaded%20PNGs/Per%20School%20Summary_Adjusted.png)

  Focusing our lens on how Thomas High School compares to others schools within the district is equally important. Prior to removing the 9th grade scores, THS was ranked second just behind Cabrera. After removing the 9th grade scores, the overall percentage fell that same 0.3% as we saw above. This adjustment did not impact this ranking as it is now tied for second with Griffin High School. These scores also bear no tangible impact on any aspects of the budget since those are not correlated to scores within this data.

*<sub>Top Five Schools Original</sub>*

![ Top Five Schools_Original.png](https://github.com/Kelfang/School_District_Analysis/blob/main/Uploaded%20PNGs/Top%20Five%20Schools_Original.png)

*<sub>Top Five Schools Adjusted</sub>*

![Top Five Schools_Adjusted.png](https://github.com/Kelfang/School_District_Analysis/blob/main/Uploaded%20PNGs/Top%20Five%20Schools_Adjusted.png)

  As previously mentioned, this data is being evaluated from several different angles. Below you will see that score performance based on school size, school type, and per student spending all remain unchanged. 

#### School Size
<sub>Scores by School Size Original</sub>

![ School Size Summary_Original.png]

<sub>Scores by School Size Adjusted</sub>

![ School Size Summary_Adjusted.png]

#### Per Student Spending
<sub>Per Student Spending Original</sub>

![ Spending Summary_Original.png]

<sub>Per Student Spending Adjusted</sub>

![ Spending Summary_Adjusted.png]

#### School Type
<sub>Scores by School Type Original</sub>

![ School Type Summary_Original.png]

<sub>Scores by School Type Adjusted</sub>

![ School Type Summary_Adjusted.png]


With these higher-level overviews, both district and school, one could interpret that removing the 9th grade score data has had nominal impact on the analysis. It also indicates that the best decision was only omitting the math and reading grades, instead of marking them as “0” or removing the students completely. 

However, with this last set of images, you will see that the absence of the 9th grade scores at THS, still leaves a notable gap when you drill down into the grade level performance. There are 1,635 students at THS, and we do not have the scores of 461 of them. This means we do not have critical insight into 28% of the school. 


#### Math Scores 
<sub>Math Scores by Grade Original</sub>

![ Math Scores by Grade_Original.png]

<sub>Math Scores by Grade Adjusted</sub>

![ Math Scores by Grade_Adjusted.png]

#### Reading Scores 
<sub>Reading Scores by Grade Original</sub>

![ Reading Scores by Grade_Original.png]

<sub>Reading Scores by Grade Adjusted</sub>

![ Reading Scores by Grade_Adjusted.png]

Additionally, since so much of school analysis is about year over year (or semester over semester) performance this gap of data will have a ripple effect for the rest of the students’ high school career. In districts across the country, teachers are evaluated based on tangible outcomes (like test scores) and student services are often tied to those same metrics. Even at a district level, there can be repercussions with state and federal funding without validated test results. 
The next step should be evaluating what can be done about this gap of data and, ultimately, put policies and procedures in place to prevent this outcome in the future. 
