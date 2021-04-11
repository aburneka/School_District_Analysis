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

As seen in the images below, the data per school, was only slightly changed with the removal of the 9th grade test scores for Thomas High School. The only scores that were changed were those for Thomas High School. 

Changes in school summary: 
* Thomas High School overall passing percentage **decreased by approximately 0.32%** 
* Thomas High School reading percentage scores **decreased by approximately 0.29%**
* Thomas High School math percentage scores **decreased by approximately 0.08%** 
* Thomas High School average math score **xx by xx**
* Thomas High School average reading score **xx by xx**

I also noticed that even though we removedd the 9th grade test scores from the data that the total student count for Thomas High School did not change from 1,635 students. Initially I thought that there must be an error in the code that was used to replace the data for Thomas High School (Steps 12-14). However we only changed the overall, reading and math percentages. Leaving the other data untouched was a stated objective in the project background. 

#### School Summary Before:

<img width="827" alt="School Summary Before " src="https://user-images.githubusercontent.com/79999761/114322669-53878000-9ad6-11eb-8583-9f5a42c96e91.png">

#### School Summary After:  

<img width="1014" alt="School Summary After " src="https://user-images.githubusercontent.com/79999761/114322434-18d11800-9ad5-11eb-9dff-bebd64d6bf7f.png">


### Thomas High School Performance 

Replacing the ninth graders' math and reading scores does not change Thomas High School's performance relative to other schools. It still remains the second top performing school for, overall passing percentage, out of the 15 city schools included in the analysis, which can be seen in the image below. 

<img width="977" alt="Screen Shot 2021-04-11 at 2 44 19 PM" src="https://user-images.githubusercontent.com/79999761/114323409-ee358e00-9ad9-11eb-9d0f-5bbd8b903894.png">

### Impact on Other Metrics

#### Scores by Grade

The scores by grade were left unchanged for grades 10-12. The only change was to the 9th grade test scores, which now show nan. 

##### Math scores by Grade: 

<img width="312" alt="Math scores by grade" src="https://user-images.githubusercontent.com/79999761/114324274-12936980-9ade-11eb-8d85-993d2a4708f5.png">

#### Reading Scores by Grade: 

<img width="339" alt="Reading Scores by Grade " src="https://user-images.githubusercontent.com/79999761/114324857-7a977f00-9ae1-11eb-95d8-a9d75d2408ec.png">

#### Scores by school spending

The scores based on spending for the schools remained unchanged, with the slight changes to Thomas High School that are outlined above. Thomas High School is in  the $630 - $644 for the Spending range per student, which remains unchanged when the numbers are rounded. 

##### Before:
<img width="1010" alt="Before Spending Summary " src="https://user-images.githubusercontent.com/79999761/114325102-386f3d00-9ae3-11eb-9dfa-06e3aec86ce8.png">

<img width="845" alt="Before Spending Per Student " src="https://user-images.githubusercontent.com/79999761/114325103-3c02c400-9ae3-11eb-9a60-551c1e7a496e.png">


##### After:
<img width="1016" alt="Summary by Spending Ranges " src="https://user-images.githubusercontent.com/79999761/114324867-926f0300-9ae1-11eb-8967-5a308eb0de47.png">

<img width="821" alt="Spending Ranges by Student " src="https://user-images.githubusercontent.com/79999761/114324876-9f8bf200-9ae1-11eb-969b-4e2e01d23ee1.png">

#### Scores by school size

Removal of the ninth grade test scores did not impact the test scores by school size. Thomas High School is considered a medium school, which remains unchanged which is apparent in the images below. 

##### Before:
<img width="760" alt="Before School Size" src="https://user-images.githubusercontent.com/79999761/114325113-4ae97680-9ae3-11eb-91a4-a52e9bf6cf49.png">

##### After: 
<img width="778" alt="Scores by School Size" src="https://user-images.githubusercontent.com/79999761/114324617-f98bb800-9adf-11eb-930c-e1caa4fdb8ee.png">

#### Scores by school type

Removal of the ninth grade test scores did not impact the test scores by school type. 

##### Before:
<img width="733" alt="Before School Type " src="https://user-images.githubusercontent.com/79999761/114325150-70768000-9ae3-11eb-9190-3dc049b6e954.png">

##### After: 
<img width="715" alt="Scores by School Type " src="https://user-images.githubusercontent.com/79999761/114324937-01e4f280-9ae2-11eb-8687-2337dcd7357c.png">

## Summary 

Replacing the Thomas High School 9th graders' test scores does not impact the data in a meaningful way. I can conclude that there is no evidence of academic dishonesty among the THS 9th grade class within the disctrict. The changes that occured in the given metrics for Thomas High School were so minor that they would not be accounted for if we were to round or format the averages and percentages. 
