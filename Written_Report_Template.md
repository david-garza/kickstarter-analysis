# Kickstarting with Excel

## Overview of Project
This project continues the analysis after Louise's play *Fever* failed to meet its goal on Kickstarter. She has asked how launch dates and / or funding goals impacted the success of other Kickstarter campaigns.

### Purpose
This analysis attempts to answer Louise's additional questions and to continue demonstrating skills in excel.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Out of 4,115 Kickstarter campaigns, 1,369 **completed** theater campaigns were analysised by month created. The data was aggregated using a pivot table to filter by parent category and year. 

Campaign outcome defined the columns and values resulting in a count of successful, failed, and canceled campaigns for each month over several years.

The plot of Theater Outcomes Based on Launch Date is provided below:
![Outcomes Based on Launch Date](/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
Using countifs(), the campaigns were parsed into $5,000 bin sizes and further parsed and counted by successful, failed, or canceled.

The counts of successful, failed, and canceled were then used to compute the percentage of successful, failed, and canceled used the total count within each $5,000 bin.

A line chart was then created using the percentages with $5,000 bins along the x-axis.

The plot of Outcomes vs Goals is provided below:
![Outcomes vs Goals](/resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
1. The best month for success is May followed by June, July, and August.
2. The worst month to start a campaign is December.
3. The failure rate is constant throughout the year at about 40 failures a month.
4. The chance for success is greater than failure or canceling.

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
