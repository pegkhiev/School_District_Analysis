# School_District_Analysis

## Background

The grades of the ninth graders at Thomas High School have been changed. The decision was to 
- Replace the ninth-grade math and reading scores from Thomas High School.
- Keep all other data associated with the ninth-grade students and Thomas High School intact.

The challenge was to prepare an analysis comparing the results replacing the 9th grade scores with NaN from Thomas High School and the original results.  

## Methodology

Using Pandas on Jupyter Notebook, the following steps were taken: 
- From the student_data_df, conditionals were applied to replace math score and reading score to zero. The two conditions were: if school_name matches "Thomas High School", and if "grade" matches "9th".  If the two conditions were met, the math_score and reading_score would be replaced by NaN
- After the relevant scores were removed, the dataframe is merged into the school dataframe. 
- Subsequent steps were performed to find out all required data. 

## Findings

### District Summary:

[Excluding Thomas High School 9th grades]
<img width = 1200 alt = "district_summary_filtered" src = https://github.com/pegkhiev/School_District_Analysis/blob/master/Challenge_Files/district_summary_formated.png>

Comparing the new summary excluding the 9th grade math and reading scores of Thomas High School, average math score dropped by 0.1, reading score remained the same; passing math %, passing reading % and overall passing % also dropped by 1% respectively. 

||Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing|
|---|---|---|---|---|---|
All Students Included|79|81.9|75|86|65|
Exclude Thomas High School 9th Grade|78.9|81.9|74|85|64|


### School Summary: 

[Excluding Thomas High School 9th grades]
<img width = 1200 alt = "per_school_summary_filtered" src = https://github.com/pegkhiev/School_District_Analysis/blob/master/Challenge_Files/per_school_summary_formated.png>

There is no change in the performance of all schools except Thomas High School. The impact of replacing 9th grade math and reading scores from Thomas High School is summarized in the table below. 

|Thomas High School|Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing|
|---|---|---|---|---|---|
All Grades Included| 83.4|83.8|93|97|91|
Exclude 9th Grade|83.4|83.9|67|70|65|

### School Ranking

[School Ranking After Thomas High School 9th Grade Scores Removed]
<img width = 1200 alt = "school_ranking_filterd" src = https://github.com/pegkhiev/School_District_Analysis/blob/master/Challenge_Files/top_schools.png>

After the replacement of 9th grade math and reading scores removed from Thomas High School, Thomas High School dropped from being 2nd in overall passing percentage to the 8th.  Griffin High School became the 2nd best school in overall passing percentage. 

### Math and Reading Scores by Grade 

[Math and Reading Score by Grade, Excluding Thomas High School 9th Grades]

<img alt = "math_score_by_grade_filtered" src = https://github.com/pegkhiev/School_District_Analysis/blob/master/Challenge_Files/math_scores_by_grade.png> <img alt = "reading_by_grade_filtered" src = https://github.com/pegkhiev/School_District_Analysis/blob/master/Challenge_Files/reading_scores_by_grade.png>

The original average math score for Thomas High School 9th grade was 83.6, while the average reading score for the 9th graders was 83.7.  After the replacement, the average scores for 9th grade were NaN respectively. 

### Scores by School Spending, School Size, and School Type 

[Scores Summary, Excluding Thomas High School 9th Grades]

<img alt = "scores_by_spending_filtered" src = https://github.com/pegkhiev/School_District_Analysis/blob/master/Challenge_Files/scores_by_spending.png>
<img alt = "scores_by_size_filtered" src = https://github.com/pegkhiev/School_District_Analysis/blob/master/Challenge_Files/scores_by_size.png>
<img alt = "scores_by_type_filtered" src = 
https://github.com/pegkhiev/School_District_Analysis/blob/master/Challenge_Files/scores_by_type.png>

The imapct of replacing 9th grade scores from Thomas High School was summarized below: 

|$630-644 Spending Range|Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing|
|---|---|---|---|---|---|
All Students|78.5|81.6|73|84|63|
Exclude Thomas High School 9th Grades| 78.5|81.6|67|77|56|

|Medium School Size (1000-2000)|Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing|
|---|---|---|---|---|---|
All Students|83.4|83.9|94|97|91|
Exclude Thomas High School 9th Grades|83.4|83.9|88|91|85|

|Charter School Type|Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing|
|---|---|---|---|---|---|
All Students|83.5|83.9|94|97|90|
Exclude Thomas High School 9th Grades|83.5|83.9|90|93|87|








