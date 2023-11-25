Readme for Project1 in Programming for Data Analysis

Author: Phelim Barry

### Introduction
The purpose of this readme is to outline the requirements for Project1 in Programming for Data Analysis and describe the methods I used to address it.

### Requirements
(detail the requirements here)


### Research Methods
(detail my approach here)

The first thing to do was to decide on a real-world phenomonen for my project. After much thinking I finally decided to base my project on the subject of new graduate salaries in Ireland. This topic as it is of interest to me as I have two children who recently graduated college and have both started working - albeit in completely different industries.

Graduate salaries tend to vary quite significantly and there is much researh and data available on this topic. Different sources tend to give different figures so finding trustworthy sources was an important aspect of my research. My primary sources of data to start to understand the phenonomen were gov.ie $^1$ and also the HEA $^2$. 

My research indicated to me that the most important factors affect a new graduate salary were the grade achieved, the location of employment after graduation, the course/area of study and also the gender of the graduate. These were then the variables I considered for my project   
| Salary |
| Grade |
| Location |
| Course |
| Gender |


#### Variable2 - grade
Starting with the variable grade, I was able to identify the overall split of grades achieved. I was also able to find the average salary by grade achieved.

#### Variable2 - area of study
Similarily, I identified the numbers and percentages of students graduating from each course/area of study. And again I was able to find the average salary by area of study.

#### Variable4 - location
HEA provide details on the salary differences across the various regions in Ireland...

#### Variable4 - gender
Gender split is 45/55 female/male however males tend to eacn on average 1,500 more...

#### Variable1 - salary
From the HEA website I was able to find the average new graduate salary in Ireland as well as the distribution of salaries. I used this information to populate the final column in the dataset with a random set of normally distributed values for salary.


(describe it here - continuous varibale measuered in etc...)


### Simulation Methods
Using a newly created dataframe, I firstly create a colume of data with sample data for the ```location``` variable and base the distribution using the % split calculated earlier. Using similar methods I populate both the ```course``` and ```grade``` columns with appropriate distributions.   

For ```salary``` I firstly populate the dataframe using ```random.randint``` to produce a range of values which are normally distributed between the max and min salariy values identified earlier in my research. Given that these values are based on the population as a whole, I then apply individual weighting for each specific variable - ```grade```, ```location``` and ```course``` to produce the final dataframe.   

The dataframe now contains simulated values for graduate salary by grade, location and course.

### References
$1$ https://www.gov.ie/en/publications/
$2$ https://hea.ie/

### Appendix

#### List of Grades
H1   
H21   
H22   
H3   

#### List of Employment Location
Dublin     
South-West   
Mid-West
Mid-East
Midlands
South-East
West
Border   

#### List of Areas of Study/Course
ICT - Information, Communication and Technology   
Eng - Engineering, Manufacturing and Construction   
HS - Human Sciences, Mathematics and Statistics   
HW - Health and Welfare   
Agr - Agriculture, Forestry, Fisheries and Vetinary   
Socs - Social Sciences, Journalism and information   
Serv - Services   
Bus - Business, Administration and Law   
Ed - Education   
Arts - Arts and Humanities

