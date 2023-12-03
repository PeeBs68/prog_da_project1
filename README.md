Readme for Project1 in Programming for Data Analysis

Author: Phelim Barry

# Table of Contents

1. [Introduction](#Introduction)
2. [Requirements](#Requirements)
3. [Research Methods](#Research_Methods)
    1. [Salary](#Salary)
    2. [Grade](#Grade)
    3. [Area of Study](#Area_of_Study)
    4. [Location](#Location)
    5. [Gender](#Gender)
4. [Simulation Methods](#Simulation_Methods)
5. [Results](#Results)
6. [References](#References)
7. [Appendix](#Appendix)


### Introduction
The purpose of this readme is to outline the requirements for Project1 in Programming for Data Analysis and describe the methods I used to complete it.

### Requirements
The purpose of this project is to create a data set by simulating a real world phenomon. Specifically:   
* Choose a real world phenomon that can be measured and for which we could collect 100 data points across at least four different variables.
* Investigate the types of variables involved, their likely distributions, and their relationships with each other.
* Synthesise/simulate a data set as closely matching their properties as possible.
* Display the newly created data set in an output cell within the notebook.


### Research_Methods
The first thing to do was to decide on a real-world phenomonen for my project. After much thinking I finally decided to base my project on the subject of new graduate salaries in Ireland. This topic as it is of interest to me as I have two children who recently graduated college and have both started working - albeit in completely different industries.

Graduate salaries tend to vary quite significantly and there is much research and data available on this topic. Different sources tend to give different figures so finding trustworthy sources was an important aspect of my research. My primary sources of data to start to understand the phenonomen were gov.ie $^1$ and also the HEA $^2$. 

My research indicated to me that the most important factors affecting a new graduate salary were the grade achieved, the location of employment after graduation, the course/area of study and also the gender of the graduate. These were then the variables I considered for my project:

| Variables| 
| --- |
| Salary |
| Grade |
| Location |
| Course |
| Gender |



#### Salary
From the HEA website I was able to find a lot of information regarding new graduate salaries in Ireland such as the average, the spread by area of study and details on the general distribution of salaries.

#### Grade
Again using data from the HEA and CSO I was able to find out details on how the grade affects the salary. I was able to identify the overall split of grades achieved as well as the average salary by grade achieved.

#### Area_of_Study
Similarily, I identified the numbers and percentages of students graduating from each course/area of study. And again I was able to find the average salary by area of study.

#### Location
For details on the location variable, I was able to use the HEA as an initial source for my research. Using this and other sources I was able to find details on the salary differences across the various regions in Ireland.

#### Gender
The HEA also provided details on the Gender split in terms of both the number of students and the salary details after graduation.



### Simulation_Methods
To simulate the data I begin by creating a list of areas of study/courses and with a for loop I cycle through that list and create individual dataframes for each one. I populate each of these dataframes with random sample data for the ```location``` variable and base the distribution using the % split calculated earlier. Next, using similar methods I populate the ```course```, ```grade``` and ```gender``` columns with appropriate distributions of data identidied earlier.   

For ```salary``` I firstly populate each dataframe using ```random.randint``` to produce a range of values which are distributed between the max and min salariy values for each course/area of study  identified earlier in my research. Given that these values are based on the population as a whole, I then apply individual weighting for each specific variable - ```grade```, ```location``` and ```gender``` to produce the final dataframes. I combine the dataframes into one using ```pd.concat```.

The data set now contains simulated values for graduate salary by grade, location course and gender allowing us to see expected salaries for any range of criteria.

Note: My initial approach was to simulate the salary variable with values to cover the full range of salaries regardless of course/area of study but this produced inaccurate results. So I refined the approach and generated the salary variable using salary ranges per course/area of study instead - hence the use of multiple dataframes.

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

