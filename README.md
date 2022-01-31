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

As illustrated in the tables below, the school summary is affected minimally by the removal of the Thomas HS 9th grade data. Besides for Thomas HS, none of the analysis changes for the other 14 schools, as is expected. Cabera HS remains at the top by overall passing with 91.33%. At the bottom of the ranking is Rodriquez HS, with under a 53% overall pass rate, even after the Thomas HS data is appended. Thomas HS moves down to the 8th ranking, no longer in the top 5 and shifting Griffin HS up to 2nd rank.

![School Summary](https://user-images.githubusercontent.com/96352625/151746154-294dac6f-26d2-4728-95cf-fe2d055da2ce.png)

![School Summary_Updated](https://user-images.githubusercontent.com/96352625/151746675-5b83ba7b-73ff-46d2-ae91-30535c708e67.png)

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Changing the 9th grade Thomas HS data with NaN has greatly affected Thomas High's overall performance relative to the other schools. Originally ranked 2nd among 15, after the changes, they are now in 8th place. Their previous overall pass rate of 90.95% kept them just above Griffin, Wilson, & Pena High Schools wich all had overall pass rates between 90.0% and 90.6%. Incredibly close behind Thomas High. After the changes, Thomas HS had an oveall pass rate of only 65%, dropping by nearly 25 percentage points.

How does replacing the ninth-grade scores affect the following:
            
- Math and reading scores by grade: The changes to average scores by grade are minimal because the data change only affected Thomas HS. Thomas HS now displays "nan" for both math and reading 9th grade averages. Other than that, the scores do not and should not change for the other schools. The tables below show the math scores by grade and are very similar; the new "nan" showing in the second table under Thomas HS 9th grade. 
        
![Original Math Scores](https://user-images.githubusercontent.com/96352625/151749775-71328a5d-9219-402e-8caa-fad21120c84d.png)
 
 
![Adjusted Math Scores](https://user-images.githubusercontent.com/96352625/151749812-47e255a3-24ac-4ed3-80c8-08cec48f291b.png)

- Scores by school spending: As you can see in the tables below, there is minimal change to the overall spending per range. THe biggest change can be seen in the $630-644 range because that is the range that Thomas HS falls into. The spending per student fell about 7% in % Passing Math, % Passing Reading, and % Overall Passing in the $630-644 range. Because the test scores were removed from the data, the averages fell and spending range calculation is impacted.

![Spending Ranges](https://user-images.githubusercontent.com/96352625/151750001-ee3faf35-b877-469e-825c-34212b1aad46.png)

![Spending Ranges_Updated](https://user-images.githubusercontent.com/96352625/151750013-64ddf6a4-90ff-4c2e-87d8-789ccf853858.png)

- Scores by school size: The biggest change to the scores by school size when the 9th grade scores are removed is to the Medium sized group. Thomas HS is a medium sized school with 1635 students. Because the percentage passing math, reading, and overall goes down with the 9th grade change, the average across the range is also negatively impacted. As seen below, the overall passing percentage for medium schools is no only 85.45% when it was previously over 91%. This nearly 6% change can also be seen % Passing Math and % Passing Reading.

        Original School Size Results
![School Size](https://user-images.githubusercontent.com/96352625/151750871-52eef730-4c0f-4efe-8d98-65c5aad75edf.png)

        Adjusted School Size Results
![School Size_Updated](https://user-images.githubusercontent.com/96352625/151750885-4684300a-ddb3-4693-8008-17da128fb41a.png)

- Scores by school type: Thomas HS is a Charter school and the change in the 9th grade data is reflected in the category. Only about a 3% change, the overall pass percentage is now only 87.20% when it was previously over 90%. % Passing Math and % Passing Reading are now at 90.33% and 93.13% respectively. The District resilts are unchanged. 

### Original School Type Results
![School Type_Updated](https://user-images.githubusercontent.com/96352625/151750909-02b8fe14-b336-425e-b7b3-d19add238110.png)

### Adjusted School Type Results
![School Type](https://user-images.githubusercontent.com/96352625/151750895-88eba402-a7a7-4ef9-a48d-6037d8a0ce06.png)

## Summary
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
