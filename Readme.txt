Project Statement
-----------------------------------------------------------------------------
Gathered from 54 user Internet profiles, the intent of this project is to demonstrate the distinguishability or indistinguishability between each user. Each subject’s profile is for a duration of 1 month. Every xlsx file contains their internet usage for the 1-month period. As one’s internet usage in theory should be consistent, it should be indistinguishable over a period time, while it should be easily distinguishable statistically speaking when compared with other subjects. It is apparent that using Python to code the project is easier to accomplish importing the necessary modules. The 54 user internet profiles would need to be read using pandas module which easily creates the data frame further to manipulated. As per requirement, three section of time windows needed for comparison to seek the least amount of user for distinguishability or indistinguishability, they are separated by 10 seconds, 227 seconds, and 300 seconds (5 minutes). 

	Afterward, using Spearman’s correlation coefficient in Python to calculate the correlation coefficient values, to find three correlation values of ra12a, r1a2b, and r2a2b, theses value means that for the correlation coefficient between subject a’s week 1 or 2 and subject b’s week 1 or 2.

	Finally, based on the PValue table calculated, we can decide that two users are distinguishable or indistinguishable from each other. When P ≤ 0.05, means that correlation coefficient calculated for Internet usage patterns for an unknown subject (say b) is significantly smaller than that for a known subject (say a) and as such “subject b” will be identified as a subject distinct from “subject a”. On the contrary, when P > 0.05, indicates that correlation coefficient calculated for Internet usage patterns for an unknown subject (say b) is not significantly smaller than that for a known subject (say a), and as such “subject b” will be identified as indistinguishable from “subject a”.  






Steps to run the project
-----------------------------------------------------------------------------

• Import necessary python libraries i.e., Pandas, Spicy, Numpy etc.
• Run App.py which is going to process the files taking useful columns i.e. doctets, Real First time packets and duration to further create the dataframe and divide it two weeks for three different windows and further write it into csv files.
• Run Spear.py to import the previously created csv and calculate the spearman’s coefficient and Z value and further the P value table for three different time windows.
• Please ensure that input and output path of the files are changed in the code.

Output
-----------------------------------------------------------------------------

• The output is contained in the zip submission named PValue.csv
• Since average number of matches(P Value greater than 0.5) is largest for 10 seconds time window thus it would not be best for authentication. For 300 secs time window number of matches is second largest thus it is not the best for authentication either. 
But for time window 227 seconds, number of matches are minimum.
Thus each user will be most distinguishable with other user. And time window 227 seconds will be best for authentication.
