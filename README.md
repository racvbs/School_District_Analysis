# School_District_Analysis
Module 4 - Challenge
## Purpose
We need to do an analysis of scores of schools in a district w/ the following data:
* A high-level snapshot of the district's key metrics, presented in a table format
* An overview of the key metrics for each school, presented in a table format
* Tables presenting each of the following metrics:
* Top 5 and bottom 5 performing schools, based on the overall passing rate
* The average math score received by students in each grade level at each school
* The average reading score received by students in each grade level at each school
* School performance based on the budget per student
* School performance based on the school size 
* School performance based on the type of school

So, we need to clean the data, corroborate data is reliable and make tables to deliver the analysis

We have to files to start:
### school_data_df
* School ID
* school_name
* type
* size
* budget
### student_data_df
* Student ID
* student_name
* gender
* grade
* school_name
* reading_score
* math_score

## Analysis
### Clean data
First, the names were been cleaned from abbreviations

```
Technical Notes:
These are the bad abbreviations deleted from names:
"Dr. ", "Mr. ","Ms. ", "Mrs. ", "Miss ", " MD", " DDS", " DVM", " PhD"
```

Second we start deleting the data of Thomas High School from 9th grade because has been manipulated, so it need to be replaced as missing values
```
Technical Notes:
There were 461 registers
```
So, this is the result:

**All registers of Thomas High School from 9th grade are "NaN", i. e. not applicable for analysis**
![image](https://user-images.githubusercontent.com/85086918/126080623-eda7aa4d-2b21-4d20-86c2-bc1ae4425b2a.png)

### Analysis
In order to have all information together we merge both tables, student and school data.

Then, I made the calculations from cleaned data and the Thomas High School of 10th to 12th grades.
This is the result (w/ format to understand numbers):

![image](https://user-images.githubusercontent.com/85086918/126080781-ba3fe9bc-645b-4a29-8f67-de1ca59071a5.png)

**Conclusion: The math and reading scores are similar, then we calculate the percentage of overall passing, that represents all students above 70 points in both scores**

Then, we have a School Summary.

** With the percentages calculated from Thomas High School without 9th grade.**
![image](https://user-images.githubusercontent.com/85086918/126080844-695770c5-081d-4c41-b11e-d37e9836418d.png)

The top five schools are:

![image](https://user-images.githubusercontent.com/85086918/126080879-de93a046-8eb0-40cf-affb-1d9b018ea8b5.png)


And the worst schools are:

![image](https://user-images.githubusercontent.com/85086918/126080890-2dd74b39-96ed-46f3-9ea8-fd30d01af5ef.png)

**Conclusion: There is a GAP of almost 40 points between the best and the worst schools, that is something the authorities of the district must work**
**Less variability could have more competitivity**

These are scores by school and the average of each:

![image](https://user-images.githubusercontent.com/85086918/126081009-b2f7b4c4-2c74-412c-a478-4e930fa9277b.png)

By budget per capita:

![image](https://user-images.githubusercontent.com/85086918/126081891-e71ff192-612e-453c-9b4d-1f3c02c1bb00.png)
**Conclusion: Budget doesn't determinate the overall passing percentage.**

And this is by size of school:

![image](https://user-images.githubusercontent.com/85086918/126081925-6180f900-257d-428e-b643-2fbe00b12b5f.png)

**Conclusion: The largest the school, the larges probability to fail in passing both subjects (math and reading)**

For school type:

![image](https://user-images.githubusercontent.com/85086918/126081933-a3bde2ee-b057-4050-adc5-8fe632989300.png)
**Conclusion: Definitely, Carter schools are better than District, it's recommendable study better practices from Carter schools and replicate them in the others.**

### Summary

1. Reading and Math scores are similar, but the passing overall passing percentage show not all students are passing both.
2. The GAP between best and worst schools are almost 40 points, it's recommendable to reduce that variability to be more competitive.
3. We need to help large schools because they have the worst overall passing percentage, the district must analyse this situation because may need more resources.
4. It's recommendable to study Carter school practices in order to replicate them in District schools and help them to be better.
5. The district need to analyze what happened with Thomas High School 9th grade scores, it's relevant to be analized. 

By Raquel Valdez
