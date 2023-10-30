# Overview of the Repository

The purpose of this repository is for Jemma Marcus-Shi and Linjie Zhu to interact with GitHub to access the files for our second project in ISA 616. 

## Project Overview
Mr. Kirk Bogard is our project's client. The client jobs for this project are to improve student development, develop external relationships for FSB, and influence job types and salary levels offered for FSB students. The client is struggling with finding trends in where students are going to work after graduation, the difference in student salaries by state. We hope to shed light on this by making a map of the US that separates job placement by city as well as average salary by state.

Our group will be using the FSB data on the employment status of graduates in order to find information about geographic trends (Question #1 in the project). We will be determining where students are going and what the salary differentials are by state where graduates most commonly work. The results of the analysis will be represented visually by graphs and maps as well as written explanation.

By understanding the data, the client can understand how each state affects students' salaries and  understand which cities are most likely to give FSB students job opportunities.

## Data Sources

We have three years of data representing FSB graduates in 2019, 2020, and 2021. The dataset provided had 42 variables. The source is either derived by Professor Jones-Farmer during data cleaning/merging, from the Oracle Business Intelligence Enterprise Edition (OBIEE) maintained by Miami administration, or from the self reported senior survey. The files have been cleaned and merged into one file.
The file name in the R project is FSB_BI_Survey_2019_2021.rds
The file name after the data cleaning is FSB_Survey.csv

## Data Description

The file we begin with has 3235 rows and 17 columns. The data that comes from the student survey has varying percentages of null variables. The variables that are most relevant to our research question are survey_city, survey_state, and survey_salary. Survey_city is missing 41% of values, survey_state is missing 40% of values, and survey_salary is missing 46% of values.

Our group will be using the FSB data on the employment location and salary of graduates in order to find information about geographic trends. The data file includes limited survey data on where students are located for their employment, what students' salaries are, and the job opportunities for Miami students that existed in different regions between 2019 to 2021.

The meaning of the columns in the datafile are as follows:

1.  nmajor: numeric,derived, the number of majors 
2.  major1: text, OBIEE, first major
3.  major 2: text, OBIEE, second major
4.  BBRJ: binary, OBIEE, an attribute of a student, but we do not know what this stands for
5.  Business Direct Admit: binary, OBIEE, a direct admit to FSB as a first year
6.  Combined Cacc and Masters: binary, OBIEE, combined degree student
7.  Dean's List: binary, OBIEE, achieve dean's list status at least once
8.  First Generation College Stdnt: binary, OBIEE, first generation student status
9.  FSB Scholars: binary, OBIEE, FSB scholars program
10.  Honors Program: binary, OBIEE, member of University honors program
11.  President's list: binary, OBIEE, achieved president's list at least once
12.  Study Abroud Courtesy Account: binary, OBIEE, do not know meaning
13.  Transfer Work: binary, OBIEE, do not know exact meaning
14.  Cum Laude: binary, OBIEE, graduated Cum Laude
15.  Magna Cum Laude: binary, OBIEE, graduated Magna Cum Laude
16.  Summa Cum Laude: binary, OBIEE, graduated Summa Cum Laude
17.  University Honors: binary, OBIEE, graduated with University Honors
18.  University Honors w/Distinction: binary, OBIEE, graduated with University Honors with Distinction
19.  minor1: text, OBIEE, first listed minor
20.  minor2: text, OBIEE, second listed minor
21.  IPEDS.Race.Ethnicity: text, OBIEE, race/ethnicity
22.  Gender: text, OBIEE, sex
23.  GPA.Range: text, OBIEE, GPA within a .5 range
24.  Term.Code: numeric, OBIEE, First four digits are the graduation year (beginning in July, e.g. July 2020 is FY 2021).  Last two digits is the term (10=fall, 15=winter, 20=spring, 30=summer).
25.  Year.x: text, derived, first four digits of Term.Code stored as a character variable
26.  latin_honors: text, survey, latin honors designation
27.  survey_city: text, survey, student reported city in which their job is located
28.  survey_company: text, survey, student reported company in which they accepted a job
29.  survey_deptfunc: text, survey, student reported job function
30.  survey_gradprogram: text, survey, student reported graduate program they will be attending
31.  survey_gradschool: text, survey, stuent reported graduate school they will be attending
32.  survey_internfour: text, survey, student reported fourth internship they held during college
33.  survey_internthree: text, survey, student reported third internship they held during college
34.  survey_interntwo: text, survey, student reported second internship they held during college
35.  survey_internone: text, survey, student reported first internship they held during college
36.  Survey_internships: text, survey, Student reported number of internships they held during college
37.  survey_offers: text, survey, student reported number of offers for full time employment received
38.  survey_plans: text, survey, student reported plans after graduation
39.  survey_pref_field: text, survey, student reported whether working in preferred field
40.  survey_pref_loc: text, survey, student reported whether working in preferred location
41.  survey_salary: numeric, survey, student reported salary
42.  survey_state: text, survey, student reported state in which job is located
