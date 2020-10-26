# School_District_Analysis Overview
---
Our client, Maria has asked to take two data sets, a smaller data set composed of data about 15 schools in the school district and a second, much larger dataset composed of detailed information about students including their names, grades, high school name, reading and math scores.  Maria has asked us to provide the following:

* A high-level snapshot of the district's key metrics, presented in a table format
* An overview of the key metrics for each school, presented in a table format
* Tables presenting each of the following metrics:
    - Top 5 and bottom 5 performing schools, based on the overall passing rate
    - The average math score received by students in each grade level at each school
    - The average reading score received by students in each grade level at each school
    - School performance based on the budget per student
    - School performance based on the school size 
    - School performance based on the type of school

The first task after downloading the data was to inspect visually and with several python functions and methods to ensure the data was clean and in the appropriate format.  It was determined that the data did need some clean-up including correcting for inappropriate prefixes and suffixes.  Following code excerpt demonstrates the cleaning method:

'''
# Cleaning Student Names and Replacing Substrings in a Python String
# Add each prefix and suffix to remove to a list.
prefixes_suffixes = ["Dr. ", "Mr. ","Ms. ", "Mrs. ", "Miss ", " MD", " DDS", " DVM", " PhD"]

# Iterate through the words in the "prefixes_suffixes" list and replace them with an empty space, "".
for word in prefixes_suffixes:
    student_data_df["student_name"] = student_data_df["student_name"].str.replace(word,"")
'''

# Results
---
# Summary

## Deliverables:
