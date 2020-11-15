# INST126-Project-3
Team Members: Dante Cavalier  

Program prompts the user to choose from a list of reports to view. 
1. suspicious_report.txt
2. irresponsible_report.txt
3. glitch_report.txt
4. domain_report.txt

If none of the avaialble reports are returned as user input it will loop again and prompt the user untill an viable input it entered. 

For each report text file there is a function to run, for which will generate the appropriate text file. 
1. suspicious_activities()
2. irresponsible_behavior()
3. system_glitch()
4. domain_count()

The suspicious_activities function will detect the number of times a user logins more than 5 times,
as well as the number of times a user logins between the times 0 or 24:00 and 5.
Each occurance will update the suspicious report counter 'sus_count'.

The irresponsible_behavior function will record the number of times a user's logins are greater than their logouts for a given day.
If the number of logins is greater than logouts that day, is recorded as one irresponsible behavior.
Each occurance of this will update the irresponsible report counter 'irres_count'.

The system_glitch function will record the number of times a user's logouts are greater than their logins for a given day.
If the number of logouts is greater than logins that day, is recorded as one system glitch.
Each occurance of this will update the glitch report counter 'glitch_count'. 

The domain_count function will read throught the original log 'userlog.log' and check record the first occurance of every domain.
These domains will be recorded in the domain report. For every line, if a domain name is repeated, that line is skipped. 
