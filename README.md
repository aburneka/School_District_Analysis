# School District Analysis
## Project Overview 

The school board believes there to be evidence of academic dishonesty, specifically with the reading and math grades for 9th graders from Thomas High School. Because the school board would like to uphold state-testing standards they have asked for additional analysis of the student data. This additional analysis requires us to replace the math and reading scores for the 9th graders from Thomas High School with NaNs while keeping the rest of the data intact. Once replaced the math and reading scores, we will repeat the school district analysis to look for any changes. 

The following data has been provided by the school board: 
* Student ID 
* Student Name 
* Gender 
* Math test scores 
* Reading test scores
* High school name 

## Resources 
* Data Sources:
  * schools_complete.csv
  * Student data: students_complete.csv
* Software: Jupyter Notebook, Pandas, Python 3.7.9, Numpy
* Other Resources for Help with Code: 
  * http://datacamp-community-prod.s3.amazonaws.com/dbed353d-2757-4617-8206-8767ab379ab3
  * https://stackoverflow.com/questions/37725195/pandas-replace-values-based-on-index
  * https://stackoverflow.com/questions/50143092/single-line-calculate-a-sum-and-print-multiple-columns-pandas-dataframe/50143235
  * https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.tail.html

## Results 

### District Summary Results  

After removing the 9th grade test scores for Thomas High School from the dataset, the disctrict summary results were not impacted in a meaningful way. Below you can see the district summary before the THS test results were removed and after: 

#### Before 

<img width="928" alt="Screen Shot 2021-04-11 at 2 33 51 PM" src="https://user-images.githubusercontent.com/79999761/114322062-18378200-9ad3-11eb-8492-2e7220495adc.png">

#### After 

<img width="786" alt="District Summary After " src="https://user-images.githubusercontent.com/79999761/114322002-ca227e80-9ad2-11eb-92ff-a4e5089e7f57.png">

### School Summary Results 

As seen in the images below, the data per school, was only slightly changed with the removal of the 9th grade test scores for Thomas High School. The only scores that were changed were thos for Thomas High School. 

Changes in school summary: 
* Thomas High School overall passing percentage decreased by approximately 0.32% 
* Thomas High School reading percentage scores decreased by approximately 0.29% 
* Thomas High School math percentage scores decreased by approximately 0.08% 
* 

#### School Summary Before:

<img width="827" alt="School Summary Before " src="https://user-images.githubusercontent.com/79999761/114322669-53878000-9ad6-11eb-8583-9f5a42c96e91.png">

#### School Summary After:  

<img width="1014" alt="School Summary After " src="https://user-images.githubusercontent.com/79999761/114322434-18d11800-9ad5-11eb-9dff-bebd64d6bf7f.png">




### Thomas High School Performance 
How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
How does replacing the ninth-grade scores affect the following:
Math and reading scores by grade
Scores by school spending
Scores by school size
Scores by school type

## Summary 
## Conclusion 
