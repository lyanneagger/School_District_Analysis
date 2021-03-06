# School District Analysis

## Overview of Project

### Purpose

This analysis uses Python to analyze standardized test data to identify performance trends around spending, grade, school, and school type. After the initial analysis, potential academic dishonesty was identified throughout the ninth grade of Thomas High School, so the analysis was run again, removing that group of students from the reporting. This report will identify the changes and comparison to the original analysis


## School District Analysis Results

- The district summary was slightly affected by removing the scores from the ninth graders at Thomas High School, as shown below. The average math score dropped by 0.1, the passing math percent dropped by 0.2%, the passing reading percent dropped by 0.3%, and the overall passing dropped by 0.1%.</br>

   District Summary including Thomas High School ninth grade scores:</br>
   ![Alt Text](https://github.com/lyanneagger/School_District_Analysis/blob/main/Resources/district_summary1.png)</br>
   District Summary after Thomas High School ninth grade scores were replaced with NaN:</br>
   ![Alt Text](https://github.com/lyanneagger/School_District_Analysis/blob/main/Resources/district_summary2.png)


- The school summary for Thomas High School was also minimally affected by removing the ninth grade scores. The largest change was in the overall passing percent, which dropped by 0.3%.

- Replacing the ninth graders' math and reading scores did not change Thomas High School's position as the second best performing school, with their overall passing percent remaining at 91%. 

Thomas High School ninth graders were also removed for the following comparisons:
- Math and reading scores were replaced with NaN for the ninth graders, but the other grades and schools were not affected.
- Scores by school spending were unaffected by removing the Thomas High School ninth graders.
- Scores by school size were unaffected by removing the Thomas High School ninth graders.
- Scores by school type were unaffected by removing the Thomas High School ninth graders.


## School District Analysis Summary

The script in the updated school district analysis has several changes. Using the `loc` function, the ninth grade math and reading scores were replaced with NaN:
```python
student_data_df.loc[(student_data_df["grade"] == "9th") & (student_data_df["school_name"] == "Thomas High School"),"math_score"]= np.nan
```

The district summary was then recalculated using the new total student count, removing the ninth grade Thomas High School students. The school summary was also recalculated to use the total number of Thomas High School tenth, eleventh, and twelfth graders. The analysis grouped by grade level within each school was also rerun to show the math and reading scores replaced with NaN for Thomas High School ninth grade students. The analyses grouped by budget, size, and type were also re-run but saw very little change since they covered multiple schools, making the sample size much larger.

The Thomas High School ninth graders had scores close to the school averages, so replacing their scores with NaN did not affect the average scores or passing percentages much. In the figures below, the average scores and passing percentages are shown to six decimal places, and the changes were minimal. The average math score dropped by 0.067412, the average reading score increased by 0.047152, the passing math percent dropped by 0.086481%, the passing reading percent dropped by 0.29013%, and the overall passing dropped by 0.317688%. Similarly, as mentioned above, the updated district summary saw similar small changes.

Thomas High School summary with ninth grade scores included:</br>
![Alt Text](https://github.com/lyanneagger/School_District_Analysis/blob/main/Resources/per_school_summary1.png)</br>
Thomas High School summary after ninth grade scores were replaced with NaN:</br>
![Alt Text](https://github.com/lyanneagger/School_District_Analysis/blob/main/Resources/per_school_summary2.png)</br>
