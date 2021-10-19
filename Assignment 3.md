## by Cristobella Durrette, Jeannie Kopstein, Zoya Mirza, and Courtney Degen

# Data 
The data our group cleaned comes from the National Center for Missing and Exploited Children and displays information for people reported missing from 1984 to 2017.

[Original data set](https://github.com/cristobella/datavisualization-fall2021/blob/2b2f674ed404254adfb2e9bc2cfb52c1837f0416/Assignment%203%20Original%20Data%20Set.csv)

[Cleaned data set](https://github.com/cristobella/datavisualization-fall2021/blob/2b2f674ed404254adfb2e9bc2cfb52c1837f0416/Assignment%203%20Cleaned%20Data.csv)


# Documentation 

You can follow along with the cleaning process in the documentation file [here](https://github.com/cristobella/datavisualization-fall2021/blob/c704eb63ce70f559453fa9335e0f907db3e8685f/Assignment%203.rd.xlsx). 


1. We began by separating the 'birthdate' column into birth date and birth time. Upon separating the data into two separate columns, we  realized that the file's creator had left the long date function on in their spreadsheet. This function provides an option to list birth time, but the spreadsheet did not display unique data for each individual. 
2. We removed the birth date column from the spreadsheet to avoid redundancy. 
3. We divided the date and time each individual was reported missing into different columns. We used the Text to Columns feature to separate not only the date from the time, but also whether the person was reported missing ante meridiem (a.m.) or post meridiem (p.m.).
4. We divided the date and time each individual was missing from into different columns. We used the Text to Columns feature to separate not only the date from the time, but also whether the person was last seen ante meridiem (a.m.) or post meridiem (p.m.). 
5. We broke the poster contact information into three different columns: one for information on the department overseeing the case; one for the state of the department posting the missing persons notice; and another for the poster's phone number. We denoted fields that did not contain information with N/A. 

# Analysis 

### Trustworthiness
This dataset is trustworthy because it displays data on missing persons gathered by a congressionally established non-profit that has worked with families, victims, law enforcement, and other entities to find people reported missing since 1984. 

### Limitations
The dataset does not contain any information about the status of each individuals' case. It is unclear from this dataset how many of the people included have been found and who remains missing. 

### Possibilities 
The dataset does not explicitly list the age for each person at the time they went missing, but this information could be calculated using their birth date and missing reported date information. 

The dataset also does not explicitly state the amount of time between when the person was last seen (missing from) and when they were reported missing. This information could be calculated by looking at the difference between the missing from and missing reported column values for each individual. 
