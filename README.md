# Kickstarting with Excel

## Overview of Project
This project continues the analysis after Louise's play *Fever* failed to meet its goal on Kickstarter. She has asked how launch dates and / or funding goals impacted the success of other Kickstarter campaigns.

### Purpose
This analysis attempts to answer Louise's additional questions and to continue demonstrating skills in excel.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Out of 4,114 Kickstarter campaigns, 1,369 **completed** theater campaigns were analysised by month created. The data was aggregated using a pivot table to filter by parent category and year. 

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
A challenge was encountered with COUNTIFS(). Most of the goal bins require an AND condition to test between to values. COUNTIFS() does not accept the excel function AND() in its criteria arguement. The only way to add boolen AND is to add the tested array again and second criteria test. This was not obvious and allows more more bugs to enter the code.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
1. The best month for success is May followed by June, July, and August.
2. The worst month to start a campaign is December.
3. The failure rate is constant throughout the year at about 40 failures a month.
4. The chance for success is greater than failure or canceling.

- What can you conclude about the Outcomes based on Goals?
1. Then general trend as goal increases is chance of success decreases. To have a channce of 50% or greater for success, goals should be $1,500 or less.

- What are some limitations of this dataset?
One huge limitation of this dataset is that the goal amounts are in different currencies. Therefore, outcomes based on goal isn't a direct apples to apples comparison among the campaigns.

- What are some other possible tables and/or graphs that we could create?
An additional Outcomes Based on Launch Date filtered on the subcategory "plays" would be helpful identifiying times of year best suited for "plays".

As mentioned above, the data should also be filtered by country to remove the bias of the different currencies.

Either a table or a chart showing the number of backers by goal bin could be informative. Especially given that the general trend of success decrease as goal increases, but there are outliers in the 35,000 and 40,000 bin that buck this trend. It may be useful to understand if they had single huge backers that made them successes.
