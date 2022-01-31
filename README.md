# School_District_Analysis
Challenge 4
## Project Overview
Maria, the Chief Data Scientist for the City School District, has hired me to analyze standardized testing scores and funding to share with the School Board and Superindent to aid budget and teaching decisions. She has tasked me with aggregating the data and showcasing trends in school performance across the district at the school and grade level. She is looking for these key data points:
- A high-level snapshot of the district's key metrics, presented in a table format,
- An overview of the key metrics for each school, presented in a table format,
- and tables presenting each of the following metrics:
    - Top 5 and bottom 5 performing schools, based on the overall passing rate,
    - The average math score received by students in each grade level at each school,
    - The average reading score received by students in each grade level at each school,
    - School performance based on the budget per student,
    - School performance based on the school size,
    - School performance based on the type of school.

However, after these results were shared with the School Board, they believe there may be evidence of academic dishonesty in the 9th Grade at Thomas High School. They asked me to re-run the analysis after replacing those scores with NaNs while keeping the rest of the data intact. The different results are explored below.
### Resources
            Data Sources: schools_complete.csv & students_complete.csv
            
            Software: Python 3.9.7
## Results
- How is the district summary affected?

Before removing the 9th grade data for Thomas HS, the average math and readings scores were 79.0 & 81.9 respectively. 75% of students passing math & 86% passing reading with an overall pass rate of 65%. After removing the 9th grade data from Thomas HS, the scores fell stlightly across the board. As you can see in the second image below, the overall pass rate is now just below the previous at 64.9%. Suggesting that removing the data did not drasticlly change the averages and scores across the whole data set.

![District Summary](https://user-images.githubusercontent.com/96352625/151735493-5ed91663-48c5-46dc-88ae-a87f1700ab93.png)

![District Summary_Updated](https://user-images.githubusercontent.com/96352625/151735500-39f1fc2d-89cc-487b-9866-46c9cc3ac3e1.png)

- How is the school summary affected?

As illustrated in the tables below, the school summary is affected minimally by the removal of the Thomas HS 9th grade data. Besides for Thomas HS, none of the analysis changes for the other 14 schools, as is expected. Cabera HS remains at the top by overall passing with 91.33%. At the bottom of the ranking is Rodriquez HS, with under a 53% overall pass rate, even after the Thomas HS data is appended.

![School Summary](https://user-images.githubusercontent.com/96352625/151746154-294dac6f-26d2-4728-95cf-fe2d055da2ce.png)

![School Summary_Updated](https://user-images.githubusercontent.com/96352625/151746675-5b83ba7b-73ff-46d2-ae91-30535c708e67.png)

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
- How does replacing the ninth-grade scores affect the following:
    - Math and reading scores by grade
    - Scores by school spending
    - Scores by school size
    - Scores by school type
## Summary
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
