# Module 4 Challenge - School District Analysis

## Project Overview

A school board requested analysis to be completed regarding academic performance metrics from different school districts and schools.  The main analysis focused on the performance of math and reading scores.  After review of the initial analysis, there appeared to be some abnormalities in the data, specifically regarding the math and reading scores from grade nine students at Thomas High School.  To further understanding these irregularities, the school board requested the analysis be repeated with the removal of the Thomas High School grade nine scores.  Both math and reading scores were replaced with "NaN" (Not-A-Number) values.  Both analyses would be compared to determine the impact of 9th grade Thomas High School reading and math scores on the overall performance of the schools overseen by the school board.

## Results

### Process and Methodology

The data used for the analysis can be accessed via the following links:

School Data - 

https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/schools_complete.csv

Student Data -

https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/students_complete.csv

The code used for the original analysis can be assessed via the following link - 

https://github.com/jbowman86/School_District_Analysis/blob/main/PyCitySchools.ipynb

The code used adjusted analysis can be accessed via the following link -

https://github.com/jbowman86/School_District_Analysis/blob/main/PyCitySchools_Challenge.ipynb

### How is the district summary affected?

The initial math and reading score analysis for the fifteen schools within the district is included below:

![
](https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/school_district_analysis_summary_original.png)


The records of 461 9th graders at Thomas High School was turned into null data, which recalculated the percentages of passing math, passing reading, and the overall passing.  The total count of students did not change as that was run on the count of the student ids, which was not turned into null data. The adjusted analysis is included below:

![
](https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/school_district_analysis_summary_adjusted.png)

When comparing the two analyses, the average math score decreased by 0.06, the average reading score dropped by 0.02 points, the percentage passing math dropped by 0.22%, the percentage passing reading decreased by 0.15%, and overall passing rate dropped by 0.31%.  Overall, the changes in scored do not appear to be substantial.

### How is the school summary affected?

The original analysis for school results can observed in the link below:

![
](https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/Thomas_High_School_original_analysis.png)

The school board was concerned that Thomas High SchoolÕs initial 90.95% overall pass rate was too high.  After calculating the total number of 10th - 12th grade students as the new denominator, the rest of the testing data was adjusted and can be obtained below:

![
](https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/Thomas_High_School_adjusted_analysis.png)

Removing the 9th grade students from the data set had a substantial impact by dropping the overall pass rate from 90.95% to 65.08% for the overall passing rate. 

### How does replacing the ninth graders' math and reading scores affect Thomas High School's performance relative to the other schools?

In the original analysis, Thomas High School ranked 2nd in the district based on overall pass rate.  The initial top five ranked schools can be seen below:

![
](https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/top_5_schools_original_analysis.png)

After adjusting the 9th grade data, Thomas High School dropped to 8th overall in terms of overall pass rate.  The bottom eight performing schools can be observed below: 

![
](https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/Thomas_High_School_ranking_adjusted.png)

The adjusting the 9th grade scores from Thomas High School scores, the school decreased its overall ranking of the school within the district from 2nd overall to 8th; thereby, removing it from the top five schools.

## How does replacing the ninth-grade scores affect the following:

### Adjusted Averages using the Math and Reading Scores 

In the original analysis, Thomas High School had 83.6 math average and 83.7 reading average for the 9th grade tests. Now the scores have been replaced with null values and shows up in Python programming as NaN in the following charts. 

Adjusted average math scores by grade and school:
![
](https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/adjusted_average_math_scores_by_grade.png)

Adjusted average reading scores by grade and school:

![
](https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/adjusted_average_reading_scores_by_grade.png)

As can be observed, the data replacement did not change the math and reading scores by grade.  

### Scores by school spending

The initial analysis of math and reading scores based on spending per student for the fifteen schools within the district is included below.  It is noted that Thomas High School falls in the $630-$644/student spending range.

![
](https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/scores_by_spending_original.png)

The adjusted analysis for math and reading scores compared to spending per student is included below:

![
](https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/scores_by_spending_adjusted.png)

The adjustment to the dataset had little impact on average math and reading scores based on spending.  However, there were differences observed when comparing spending ranges to passing percentages.  It was found that there was a 0.02% drop in percentage passing math, a 0.07% decline in percentage passing reading, and a 0.08% decrease in percentage passing overall among schools spending $630-644 per student.

### Scores by school size

Analysis for schools based on size was conducted by grouping schools based on their number of total students.  Small schools had less than 1000 students, medium schools had between 1000 and 2000 students and large schools had more than 2000 students.  Thomas High School is defined as a medium sized school.  The initial analysis for math and reading scores based on school size are presented below:

![
](https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/scores_by_school_size_original.png)

The adjusted analysis for math and reading scores based on school size is included below:

![
](https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/scores_by_school_size_adjusted.png)

When adjusted for Thomas High School 9th grade results, there was no change in the average math or reading scores for medium sized schools.  However, there was small changes to the percentage passing math, reading and overall.  In the adjusted analysis, the percentage of students passing math dropped 0.02%.  Additionally, the percentage of students passing reading decreased by 0.06%.  Lastly, the overall passing percentage declined by 0.06%.  The scores for the small and large schools were unaffected by the adjustments made to the data for this analysis.

### Scores by school type

The math and reading scores between charter and district schools were compared.  Thomas High School is a charter school type. The initial analysis results can be seen below:

![
](https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/scores_by_school_type_original.png)

The adjusted analysis for math and reading scores by school type is included below:

![
](https://github.com/jbowman86/School_District_Analysis/blob/main/Resources/scores_by_school_type_adjusted.png)

There was no change in average math and reading scores for charter schools after adjusted from Thomas High School 9th grade scores.  Removing the 9th grade scores from Thomas High School did lead to a 0.01% decline percentage passing math, a drop of 0.04% in percentage passing reading and a 0.04% decline in overall passing percentage among students at charter schools.  This analysis had no impact on the results obtained from district schools.

## Summary: Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

1. The overall passing rate for Thomas High School changed dramatically from 91% to 65%. 

2. Thomas High School's ranking dropped from 2nd to 8th in the district of 15 campuses. 

3. Percentage of students at medium sized schools who received passing math, reading, and overall scores were seen to decrease by less than 0.1 percentage points across all three measure.

4. Charter schools performed substantially better than district schools (90.43% vs. 53.67% overall pass rate).  These changes were maintained even when removing the Thomas High School 9th grade scores (90.39% vs. 53.67% overall pass rate).
