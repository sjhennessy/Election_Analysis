# Election_Analysis
## Overview of Election Audit
The purpose of the election audit analysis is to help Tom, a Colorado employee, to audit the results of an election of a congressional district in Colorado. The code and written report will certify the election results for Tom. Additionally, the python code used for the Colorado congressional district could be used for other local elections in the future.

## Election-Audit Results
### How many votes were cast in this congressional election?
    Total Votes: 369,711

### Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.
    County Votes:
    Jefferson: 10.5% (38855)
    Denver: 82.8% (306055)
    Arapahoe: 6.7% (24801)

### Which county had the largest number of votes?
    Largest county turnout : Denver

### Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
    Charles Casper Stockham: 23.0% (85,213)
    Diana DeGette: 73.8% (272,892)
    Raymon Anthony Doane: 3.1% (11,606)

### Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
    Winner: Diana DeGette
    Winning Vote Count: 272,892
    Winning Percentage: 73.8%

## Election-Audit Summary

To the election commission:
The purpose of this proposal is to offer the script written for the county election in Colorado as a general script for any election in Colorado. By modifying a small amount of code, elections of any size could be analyzed quickly and accurately. There are two examples below that explain modifications to the script that could be used for upcoming elections in Colorado.

### In line 17 and 18 of the PyPoll_Challenge_FINAL.py code, 
    county_votes = {}
    county_list = []
the variables which contain the word "county" could be replaced with another variable such as "state_votes" for a national election such as a presidential election, or "town_votes" for a state election.

### Another example of how the script can be modified is to show the Loser in the election rather than the Winner. The variables listed below would be exchanged with the 'losing variables': 

#Initialize winning variables
    winning_candidate = ""
    winning_count = 0
    winning_percentage = 0

The word "winning" would then be replaced with "losing" and the code for determining vote count would be 'less than' rather than 'greater than' in line 151.