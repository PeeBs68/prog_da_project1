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

#### Variable1 - salary
From the HEA website I was able to find the average new graduate salary in Ireland. 
(describe it here - continuous varibale measuered in etc...)


(move this bit to below somewhere)
Combining details from both gov.ie and HEA I was able to calculate the average salary across the different regions broken down by both industry sector and grade achieved...

#### Variable2 - grade
gov.ie also shows the average salary by grade achieved...

#### Variable2 - area of study
gov.ie also shows the average salary by area of study...

#### Variable4 - location
HEA provide details on the salary differences across the various regions in Ireland...

### Simulation Methods
Using a newly created dataframe, I firstly create a colume of data with sample data for the ```location``` variable and base the distribution using the % split calculated earlier. Using similar methods I populate both the ```course``` and ```grade``` columns with appropriate distributions.   

For ```salary``` I firstly populate the dataframe using ```random.randint``` to produce a range of values which are normally distributed between the max and min salariy values identified earlier in my research. Given that these values are based on the population as a whole, I then apply individual weighting for each specific variable - ```grade```, ```location``` and ```course``` to produce the final dataframe.   

The dataframe now contains simulated values for graduate salary by grade, location and course.

### References
gov.ie
HEA
etc