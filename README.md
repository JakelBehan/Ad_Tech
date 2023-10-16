# Ad_Tech_Challenge

The purpose of the following analysis is to demonstrate skills in data management, analytical ability, business strategy, and communications skills. This challenge was given to real life applicants in order to test these very skills for a role within the ad tech industry. I have chosen to do this challenge in order to demonstrate my own skills and develop my knowledge of ad tech. The full details of the challenge can be read in the file titled SBM 2017 Analytics Challenge.pdf.

# Preparing and processing

We were given real data that Chegg has received from its ad partners in a csv file. The file contains the following, DFP Impressions, Paid Impressions, DFP Revenue, and Ad Revenue. Each row contains these values for each respective ad partner along with the date the data was received and the website it was collected from. To begin the cleaning process the project dataset was copied to ensure a backup is available. Each column was then checked for consistent formatting. To begin this process filters were created to see if any inconsistencies existed in the date column. No blank cells existed however a few instances of “Total” existed. We find in these “total” rows the metrics for each month are summed. This is irrelevant and causes inconsistent formatting so these rows were removed. Next the site column was checked for inconsistencies by filtering. No instances of incorrect formatting or spelling was detected. The rest of the columns contain only numbers so filtering won't be ideal for checking consistent formatting. To check that each cell is a number we create a new sheet that references each column using an array function. The function then fills each corresponding cell it references with text stating “Valid Number” or “Not Number”. We then filter each of these columns to see if any instances of “Not Number” appear. We also double check the date column using the same technique. The date column returns “Valid date” or “Not a date”. No instances of “Not Number” or “Not a date” appear. The last concern was many instances of zero or empty values in the number columns. This means no value was reported and is detailed in the project description. Too many instances of empty values appear to remove rows where they occur. With the formatting checked, a pivot table is created that sums the values of all three sites on each corresponding date. The “Mth” column was not included due to its irrelevance. Snorlax Tagless was also excluded because every cell was empty besides 2 that had a value of 11 in the DFP revenue column. These cells were removed in the early stages of the cleaning process but can be seen in the backup sheet. All of the tables mentioned can be seen in the table folder.

# Analysis

After creating a clean pivot table, the calculator was made in a new sheet. The calculator can also be seen within the table folder. The date cell is referenced by every function and looks up data from the pivot table. Changing the date calculates the specific metrics for the seven days leading up to and including the date refenced. The weeks where many instances of no values were reported causes a bit of trouble for the calculator, for example #DIV/0!. However the dates required of the project work fine along with weeks that don't have any missing data. Visualizations were also created using data from the calculator that display revenue and impression metrics for each ad partner. The google sheets versions of the tables can be seen here https://docs.google.com/spreadsheets/d/1csLt4v4wTiBpHGECP6MoMn3YKTRv6sHdd_T5IsLsbpQ/edit?usp=sharing

# Share

A Presentation utilizing the charts and insight gathered was made in Google Slides. It Details the findings and gives recommendations on how to move forward given the business task. The presentation is linked here https://docs.google.com/presentation/d/1DI1JOxZI_r1kTynEBCx_z_kvH_Q18wEevoof3Pio5dI/edit?usp=sharing

# Other

The second part of this challenge asks to respond to a real life situation while detailing the process and response to the scenario. The details of part two can be seen in the SBM 2017 Analytics Challenge.pdf. The Response can be seen in the Ad_Tech_Challenge_Part_2.pdf
