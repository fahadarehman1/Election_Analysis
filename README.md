# 							Election Audit - Python 

## Overview of Election Audit

Assist Colorado Board of Election employee(Tom) with an election Audit. The data is from congressional district office with the key emphasis on three counties

The first ask is to deliver the following data elements (Total no. of votes, Candidate list, Candidate votes received, Candidate votes percentage, and the Election's winner)

The additional ask is to enhanced the script and add the additional following elements(Voter turnout of each county, Percentage of voters turnout from each county, and the county with the highest turnout)

Certify the election results and present it to the board

#### 	Data and Coding Criteria:

- Scope is only for DRE computer counted data and not 'hand counted' or 'machine counted' method 
- Code will be created in Python
- Python code will read data from csv file and write a text file out
- Data is available in the csv format
- First column of the csv column is header which is excluded from if/else, for loop statements
- Code and related files will be uploaded on GIT and maintained in GIT for version controlling 

## **Election-Audit Results:** 

Using the Python code, we can answer the following questions and audit the answers with the output from the code provided below

- How many votes were cast in this congressional election? 

  - ###### 369,711 votes casted

- Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.

  - ###### Jefferson: 10.5% (38,855)

  - ###### Denver: 82.8% (306,055)

  - ###### Arapahoe: 6.7% (24,801)

- Which county had the largest number of votes?

  - ###### Denver

- Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.

  - ###### Charles Casper Stockham: 23.0% (85,213)

  - ###### Diana DeGette: 73.8% (272,892)

  - ###### Raymon Anthony Doane: 3.1% (11,606) 

- Which candidate won the election, what was their vote count, and what was their percentage of the total votes?

  - ###### Winner: Diana DeGette , Vote Count: 272,892 , Percentage: 73.8%

![Output from the code as an supporting document](/Resources/Elections_Screen_Snippet.PNG)



## Election-Audit Summary

We were able to automate this process as much as possible and provide the final results to Colorado Election Commission for certification and audit results. The same script can be used for regional and city elections as well as for senate elections if needed. 

In order to use this script for any other elections, the input file variable and the output file variable needs to be updated. The candidate name is coming from column C and county is coming from column B, as long as the new data points are in the same columns then we just have to update the variable names and the output print statements. If the new data is in some other columns then we have change the index in code: candidate_name = row[2] or county_name = row[1] to the appropriate index. Remember index starts at position 0(zero).

If more than two data points are being analyzed, then we need to initialize the variables and try to mimic the same code that we have created for candidate and counties. The basic structure remains the same. 

