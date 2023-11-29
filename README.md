Readme for Project1 in Programming for Data Analysis

Author: Phelim Barry

# Table of Contents

1. [Introduction](#Introduction)
2. [Requirements](#Requirements)
3. [Research Methods](#Research Methods)
    1. [Salary](#salary)
    2. [Grade](#grade)
    3. [Area of Study](#Area of Study)
    4. [Location](#location)
    5. [Gender](#gender)
4. [Simulation Methods](#Simulation Methods)
5. [Results](#Results)
6. [References](#References)
7. [Appendix](#Appendix)


### Introduction
The purpose of this readme is to outline the requirements for Project1 in Programming for Data Analysis and describe the methods I used to address it.

### Requirements
The purpose of this project is to create a data set by simulating a real world phenomon. Specifically:   
* Choose a real world phenomon that can be measured and for which we could collect 100 data points across at least four different variables.
* Investigate the types of variables involved, their likely distributions, and their relationships with each other.
* Synthesise/simulate a data set as closely matching their properties as possible.
* Display the newly created data set in an output cell within the notebook.


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

#### Variable3 - area of study
Similarily, I identified the numbers and percentages of students graduating from each course/area of study. And again I was able to find the average salary by area of study.

#### Variable4 - location
HEA provide details on the salary differences across the various regions in Ireland...

#### Variable5 - gender
Gender split is 45/55 female/male however males tend to eacn on average 1,500 more...

#### Variable1 - salary
From the HEA website I was able to find the average new graduate salary in Ireland as well as the distribution of salaries. I used this information to populate the final column in the dataset with a random set of normally distributed values for salary.


(describe it here - continuous varibale measuered in etc...)


### Simulation Methods
Using a newly created dataframe, I firstly create a colume of data with sample data for the ```location``` variable and base the distribution using the % split calculated earlier. Using similar methods I populate both the ```course``` and ```grade``` columns with appropriate distributions.   

For ```salary``` I firstly populate the dataframe using ```random.randint``` to produce a range of values which are normally distributed between the max and min salariy values identified earlier in my research. Given that these values are based on the population as a whole, I then apply individual weighting for each specific variable - ```grade```, ```location``` and ```course``` to produce the final dataframe.   

The dataframe now contains simulated values for graduate salary by grade, location and course.

### Results
In our results section we use a range of statistics and graphs to visualise the new data set. We also verify that the new data matches the characteristics of the original data.

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

