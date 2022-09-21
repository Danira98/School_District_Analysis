# ***School District Analysis with Pandas***

## Project Overview:

### Overview:

A chief data scientist of a city school district gave us the task to analyze student funding and students' standarized test scores to report back trends and patterns in school performance. We will be looking at both Charter and Public schools, focusing on the grades of 9 through 12 individually, and its reading and math scores.

### Purpose:

In this project, we are instructed to use Pandas to fastrack our analysis,clean our data and aggregate the data given for reading scores and math scores of both Charter and Public schools. We will return a report containing the trends of each school for these subjects, report back statistics for certain grades, and taking a look at the budget given for each school.

## Results:

### Code:
In order for us to return accurate data, we first needed to clean our data of duplicates and null/missing values. We achieved this by first checking if there were any null values in our Data Frame and then remove the rows with the columns that contain those values. We do the same process with the duplicated rows. The following code shows these steps:

```
# Check for null values
student_df.isnull()

# Drop rows with null values and verify removal
student_df = student_df.dropna()
student_df.isnull().sum()
```
Next

Add stuff


### Results:

From our analysis, we could gather the following results:
- The average reading score of all grades between Charter and Public schools is 72.36 .
- The average math score of all grades between Charter and Public schools is 64.68 .

![describe function for all grades](https://user-images.githubusercontent.com/111034667/191600701-dbd8563c-d1d9-4647-a389-c38527360f17.png)

<sub> Statistics Summary for all data <sub>
  
- The average reading score for all grades in the Charter schools is 72.45 while the average reading score for all grades in the Public schools is 72.28
- The average math score for all grades in the Charter schools is 66.76 while the average math score for all grades in the Public schools is 62.95
  
  ![Averages for reading and math scores(All Schools_Grades)](https://user-images.githubusercontent.com/111034667/191601464-9c4ad263-46bb-4414-ac24-7f7a5626b52b.png)

  <sub> Averages for reading and math scores  (all grades) <sub>
  
  
- The grade with the highest average math score in Charter schools is 9th grade
- The three grades with equal, highest average math score in Public school are 9,10 and 12 grade.
  
  ![Average math scores of each grade](https://user-images.githubusercontent.com/111034667/191601886-e841d069-179b-49c6-bfe6-58e80af4c862.png)

   <sub> Average math scores of each grade <sub>
     
  - The budget given to Charter schools in total was  $ *872,625.66* while the budget given to Public schools in total was  $ *911,195.56* .
     
     ![School Budget](https://user-images.githubusercontent.com/111034667/191603479-0f49d6c1-a88e-4ce5-aca5-f843e290d882.png)

## Summary

Overall, the Charter schools performed better in the subjects of English and Mathematics. Although their budget was smaller than Public schools, they were able to perform better.
     
The trend that is predominant with our analysis is that grade 9th overall has the highest math score accross the district,although the average is roughly a C-.Similarly with reading scores, througout the grades the average is 72, which is still low.
     
Furthermore, there is a significant drop in the math scores for 12 grade in Charter schools, and in general, the average of math scores declines in both schoools with each passing year. It would be ideal to further analyze what has caused for the math scores to drop after 9th grade in both schools, and see what needs to be done to aid students to improve their scores. Additionally, It would be helpful to review what the budgets provided are going towards to see where the district would need to increase their funding to improve grades overall


