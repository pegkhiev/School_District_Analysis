# School_District_Analysis

## Background

The grades of the ninth graders at Thomas High School have been changed. The decision was to 
- Replace the ninth-grade math and reading scores from Thomas High School.
- Keep all other data associated with the ninth-grade students and Thomas High School intact.

The challenge was to prepare an analysis comparing the results excluding the 9th grade scores from Thomas High School and the original results.  

## Methodology

Using Pandas on Jupyter Notebook, the following steps were taken: 
- From the student_data_df, conditionals were applied to replace math score and reading score to zero. The two conditions were: if school_name matches "Thomas High School", and if "grade" matches "9th".  If the two conditions were met, the math_score and reading_score would be replaced by 0
- After the relevant scores were removed, the dataframe is merged into the school dataframe. 
- Subsequent steps were performed to find out all required data. 

## Findings

### District Summary:
<img width = 600 alt = "district_summary_all_schools" src = 
