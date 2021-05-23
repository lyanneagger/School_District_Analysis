# School District Analysis


For this part of the Challenge, write a report that summarizes your updated analysis and compares it with the results from the module.

## Overview of Project

### Purpose

This analysis uses Python to analyze standardized test data to identify performance trends around spending, grade, school, and school type. After the initial analysis, potential academic dishonesty was identified throughout the ninth grade of Thomas High School, so the analysis was run again, removing that group of students from the reporting. This report will identify the changes and comparison to the original analysis


## School District Analysis Results

- The district summary was not really affected by removing the ninth graders from Thomas High School. The average math score dropped by 0.1, the passing math percent dropped by 0.2%, the passing reading percent dropped by 0.3%, and the overall passing dropped by 0.1%.

- The school summary for Thomas High School was also minimally affected by removing the ninth grade scores. The largest change was in the overall passing percent, which dropped by 0.3%.

- Replacing the ninth graders' math and reading scores did not change Thomas High School's position as the second best performing school, with their overall passing percent remaining at 91%.

Thomas High School ninth graders were also removed for the following comparisons:
- Math and reading scores were replaced with NaN for the ninth graders, but the other grades and schools were not affected.
- Scores by school spending were unaffected by removing the Thomas High School ninth graders.
- Scores by school size were unaffected by removing the Thomas High School ninth graders.
- Scores by school type were unaffected by removing the Thomas High School ninth graders.


## School District Analysis Summary

Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

The Thomas High School ninth graders had scores close to the school averages, so replacing their scores with NaN did not affect the average scores or passing percentages much. In the figures below, the average scores and passing percentages are shown to six decimal places, and the changes were minimal. The average math score dropped by 0.1, the passing math percent dropped by 0.2%, the passing reading percent dropped by 0.3%, and the overall passing dropped by 0.1%.

![Alt Text](https://github.com/lyanneagger/School_District_Analysis/blob/main/Resources/per_school_summary1.png)</br>
![Alt Text](https://github.com/lyanneagger/School_District_Analysis/blob/main/Resources/per_school_summary2.png)