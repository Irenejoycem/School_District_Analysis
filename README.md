# School_District_Analysis
Python, Pandas

# Overview of the school district analysis: 
>For this project, I analyzed data from a school district. In order for the school to properly allocate expenses for schools, I had to calculate average math and reading scores per school. I was also able to compare the type of schools, size of each school and budget for each school to see what each result was so that the district can base what the next year's budget will be.
# Results: 
Using bulleted lists and images of DataFrames as support, address the following questions.

- How is the district summary affected?
- How is the school summary affected?
- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
- How does replacing the ninth-grade scores affect the following:
- Math and reading scores by grade
- Scores by school spending
- Scores by school size
- Scores by school type

# Summary: 
>Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

After making all the proper calculations from the original data, I then had to remove all of Thomas High School's 9th grade scores due to academic dishonety. I was able to use the code

```student_data_df.loc[(student_data_df["grade"] == "9th") & (student_data_df["school_name"] == "Thomas High School"),"reading_score"]=np.nan```

and

```student_data_df.loc[(student_data_df["grade"] == "9th") & (student_data_df["school_name"] == "Thomas High School"),"math_score"]=np.nan```
to remove all of the 9th grade Thomas High School scores and replaced them with a NaN (not a number).

Four major changes from the original calculations were the math score percentage, reading score percentage, overall score percentage and total number of students counted for the analysis.

