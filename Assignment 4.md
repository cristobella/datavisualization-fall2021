# Assignment 4: Data Cleaning and Analysis


## 1a. Link to the dataset: [Supplementary Homicide Report](http://www.murderdata.org/p/data-docs.html) 


## 1b. Questions and answers

### -Q: In which states do you see the longest and shortest average delay between a homicide and its case filing? 

  -A: Iowa, Idaho, and South Carolina have the longest average delay, while Washington, D.C., Nevada, and Maryland have the shortest average delay.
  
### -Q: In which states are cold case homicides most and least likely to be a result of gun violence? 

  -A: Louisiana, Washington, D.C., and Mississippi are the most likely states for a homicide to be a result of gun violence, while Hawaii, South Dakota, and New Hampshire are the least likely states for a homicide to be a result of gun violence.
  
### -Q: What demographic of victims (with 100 or more sample size) is most likely to be a victim of homicide from a stranger? 

  -A: Homicides of Asian male victims were most likely to have been committed by offenders who were unknown to the victim. 
  
  
  ## 2. Data cleaning (see separate file) 
  
  1. I substituted 999 for N/A in the "VicAge" column.
   
  2. I substituted 999 for N/A in the "OffAge" column. 
  
  3. I added the "Stranger" column to show victims' relationship to their assailant using an =IF statement formula. The formula returns YES if the perpetrator was a stranger to the victim and NO if the perpetrator was not a stranger to the victim. 
   
  4. I altered the format of the date in the "FileDate" column.
  
  5. I found the "MonthValue" from the "Month" column to create consistency across dates in the data set. 
   
  6. I combined month and year values to display the incident date and to create consistency across dates in the data set. 
  
  7. I changed the format of the date in the "IncidentDate" column, adding ones as placeholders for the day of the month because that data was not provided.
   
  8. I removed superfluous columns. 
   
  9. I calculated the file lag time using the formula =DAYS(AC#, I#) to find the number of days between when an incident occurred and when a report on the incident was filed with law enforcement. 
   
  10. I wrote a formula to find which homicides involved gun violence. Drawing on data from the "Weapons" column, I extracted whether a homicide involved a gun. 
   
  11. For Question 1, I constructed a PivotTable with the "State" column under Rows and the average file lag time under "Values" column to see which states have the longest and shortest average delay between a homicide and its case filing.
   
  12. For Question 2, I constructed a PivotTable with "State" and "Gun Violence" under Rows and "Count of ID" under Values to find out what percentage of cases in a state included gun violence and what percentage of cases in a state did not include gun violence. Then, I constructed a second PivotTable to calculate the percentage of cases involving gun violence in each state. Lastly, I filtered the table from largest to smallest to determine what states' cases were the most or least likely to involve gun violence. 
    
  13. For Question 3, I constructed a PivotTable with "Sample Size" Under Filters, "Demographic" under Rows, and "Average of Stranger Violence Percentage" under Values. This allowed me to see what demographic of victim, with 100 or more for the sample size, is most likely to be a victim of homicide from a stranger. 
  
  
  ## 3. Headline and nut graph
  
  -Headline: Asian Male Homicides Most Likely to Involve Strangers, FBI Data Finds.
  
  -Nut graph: Information gathered between 1976 and 2020 shows that cases with Asian male victims age 70 or older faced the highest likelihood of stranger violence, with 34% of cases committed against that demographic involving a person unknown to the victim. 
  
  
  
