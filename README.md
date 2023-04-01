# 21479_5_Admissions
This project was carried out with the goal of creating a database for Admissions Offices. Originally, the plan was to create a functional database for one admissions office, but with creating two extra entities this database has expanded into being useful for multiple universities trying to admit their potential first year students.

## Authors
- David Adams [@dra27013](https://github.com/dra27013)
- Olivia Chaewon [@cwon-kang](http://github.com/cwon-kang)
- Spencer Gorgon [@spencergordon16](https://github.com/SpencerGordon16) 
- Erin O'Dea [@erinodea](https://github.com/erinodea/SQLgroupProj1)
- Kenneth Johnson [@kmj07215](https://github.com/kmj07215) 

## Data Model
![Logo](https://raw.githubusercontent.com/cwon-kang/armyGreen/main/dm.png)


The admissions data model contains ten key entities. Admissions office is related to University with a one to one relationship. This signifies that each University that uses this database will be associated with their own Admissions Office. The office itself has many employees. These Employees have many workers that report to a head of the Admissions office. From employees they conduct many reviews on applications and participate in many interviews as part of the application process. These applications have many interviews that take place. This creates a many-to-many relationship between application and employees connecting the two entities. High schools from around the United States have many students who will be creating many applications to get into their University of choice. Each of these students have one transcript and standardized test results connected to their information. Having all of these factors connected to each other creates an interconnected data model that portrays the admissions process of student applications.

## Data Dictionary

[DATA DICTIONARY.pdf](https://github.com/dra27013/GroupProject_Admissions/files/11123364/DATA.DICTIONARY.pdf)

## Data Dictionary 
![Logo](https://github.com/cwon-kang/armyGreen/blob/main/DATA%20DICTIONARY%20as%20img_Page_1.png?raw=true)
![Logo](https://github.com/cwon-kang/armyGreen/blob/main/DATA%20DICTIONARY%20as%20img_Page_2.png?raw=true)
![Logo](https://github.com/cwon-kang/armyGreen/blob/main/DATA%20DICTIONARY%20as%20img_Page_3.png?raw=true)
![Logo](https://github.com/cwon-kang/armyGreen/blob/main/DATA%20DICTIONARY%20as%20img_Page_4.png?raw=true)
![Logo](https://github.com/cwon-kang/armyGreen/blob/main/DATA%20DICTIONARY%20as%20img_Page_5.png?raw=true)


## Query 1:  What is the admission rate of schools that are in California?
![Logo](https://github.com/SpencerGordon16/MIST4610-Group-Project/blob/main/Screenshot%202023-03-31%20145616.png?raw=true) 

Justification: This query can be used to find the admission rate of schools within a certain state, more specifically California. There are multiple Universities in this data model that are in the state of California school system with the name that includes “University of California”. Thus, this could be useful in comparing the admission rates of schools in different states.

## Query 2: Each Dean of Admissions personally reviews a few applications: list the Dean of the Admissions Office for each School, their personal Admission Rate and how many applications they personally reviewed, admitted, deferred, and rejected. Order the results by Admission Rate ascending.
![Logo](https://github.com/SpencerGordon16/MIST4610-Group-Project/blob/main/Screenshot%202023-03-31%20124036.png?raw=true)

Justification: For each University’s Admissions Office, different employees review different applications. Thus, different employees have their own admission rates based on their decisions. This query allows for the Admissions Office to see the admission rates of their most executive employee: the Dean. It shows this for each school so they can compare the difficulty and variability of the review decisions for the Deans of each University’s Admissions Office.

## Query 3: How many interviews did a university conduct in the month of November?
![Logo](https://github.com/erinodea/SQLgroupProj1/blob/main/Screen%20Shot%202023-03-31%20at%2012.35.16%20PM.png?raw=true)

Justification: This procedure will allow for Universities to see their history of when they gave interviews. It could be altered to see any month, as well. This could be useful for scheduling future interviews and seeing historical trends when admissions offices had their busiest months.

## Query 4: List the Employees who oversee other employees and how many employees that individual oversees.
![Logo](https://github.com/erinodea/SQLgroupProj1/blob/main/Screen%20Shot%202023-03-31%20at%2012.39.21%20PM.png?raw=true)

Justification: This will allow universities to see which employees who work in the Admissions Office oversee others. This could indicate that they are a manager or head of the office, and other employees that work at the university could refer to this person for questions about admissions.

## Query 5: What is the number of students who applied to a given university with GPA’s higher than 3.5? 
![Logo](https://github.com/cwon-kang/armyGreen/blob/main/q6.png?raw=true)
Justification: It may be useful to see the number of applicants of a given university who have a GPA above 3.5 to gauge the rigor of given universities. A GPA of 3.5 can be used as an academic standard for some schools, so more students may apply to certain schools depending on their GPA. 

## Query 6: How many students in each highschool who applied Early Action have GPA’s higher than their highschool’s average GPA? 
![Logo](https://github.com/cwon-kang/armyGreen/blob/main/q5.png?raw=true)

Justification:  The rates for Early Action are slightly different from other application types. Through these results, one could assess if this has to do with whether it has to do with the number of applicant above their highschool body’s average.

## Query 7: What are the names of the students, the highschool, and the students ACT and SAT scores for those that have a higher average in both their ACT and SAT score than their respective highschool? 
![Logo](https://github.com/kmj07215/MIST-4610-GROUP-PROJECT-1/blob/main/Q7.png?raw=true)
Justification: This will show the students with above average testing scores and see how they compare from highschool to highschool.

## Query 8: How many interviews were conducted by an employee that has at least one other employee under them. 
![Logo](https://github.com/kmj07215/MIST-4610-GROUP-PROJECT-1/blob/main/Q8.png?raw=true) 

Justification: This shows that the supervisors are involved in the interviewing process for students interested in their university. 


## Query 9: List the names of students, their highschool IDs, and what their SAT Scores are in descending order depending on their application type.
![Logo](https://github.com/SpencerGordon16/MIST4610-Group-Project/blob/main/Screenshot%202023-03-31%20130724.png?raw=true)  

Justification: This way we can determine the strength of early admission students standardized test scores.

## Query 10: Determine which students from their respective high schools have a cumulative GPA that is less than 2.0. 
![Logo](https://github.com/kmj07215/MIST-4610-GROUP-PROJECT-1/blob/main/Q10.png?raw=true) 

Justification: This limits requirements by Universities for minimum GPAs.


## Query Matrix
![Logo](https://github.com/SpencerGordon16/MIST4610-Group-Project/blob/main/Screenshot%202023-03-31%20125930.png?raw=true) 
 
