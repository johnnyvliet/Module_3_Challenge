# Module_3_Challenge
**Overview of Election Audit**
The purpose of this Election Results audit was to count the votes in Jefferson, Denver and Arapahoe counties to determine the winner of the election and find the county with the largest voter turnout

**Election Audit Results**

- How many votes were cast?: A total of 369,711 votes were counted
- The count and percentage of votes in each county are as follows: Jefferson (38,855 / 10.5%), Denver (306,055 / 82.8%), Arapahoe (24,801 / 6.7%)
- Denver had the largest number of votes
- The count and percentage of votes for each candidate are as follows: Charles Casper Stockholm (85,213 / 23.0%), Diana DeGette (272,892 / 73.8%), Raymond Anthony Doane (11,606 / 3.1%)
- The winner of the election was Diana DeGette (272,892 / 73.8%)
- Here is a summary of the election results [Election Results]("C:\Users\jvanv\Election_Analysis\analysis\election_results.txt")

**Election Audit Summary**

This script was able to count the total amount of votes in three different counties and output the winner in a matter of seconds. This same algorithm can easily be reused for future elections by making small adjustments to the code. Examples of two changes are below:
- Any .csv file can be read into the code if its saved in the same folder. All that needs to change is updating the "Election_Results" at the end of this line to the name of the new list: `file_to_load = os.path.join("Election_Analysis","Resources", "election_results.csv")`
- This algorithm doesn't have to just be for county elections, it could be run for the entire state or just a school board election. The counties listed in the output come from the .csv file that's loaded into the system, but the headers in the output can be whatever the user writes. For example, if this data was from a vote for a Department of Intenal Affairs president, this line of code `f"County Votes:\n")` inside the election_results variable can be retyped as f"DIA Votes:\n" and the output would reflect this change.
