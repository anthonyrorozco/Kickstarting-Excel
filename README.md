### Kickstarting-Excel[resources.zip](https://github.com/anthonyrorozco/Kickstarting-Excel/files/8922717/resources.zip)

## Overview of Project
### Purpose

This project investigates various Kickstarter campaigns and how they performed in terms of launch dates and funding goals.

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date

The Parent Category and Years columns were used to create a pivot table. Then, within the pivot table, I filtered the Parent Category by Theater to examine the theater category. Finally, I used the pivot table to create a dotted line chart to show the relationship between outcomes and launch month.
I used the YEAR() function to extract the year from the Date Created Conversion column and placed the data in a new column, Years, to create the Years column. I then filtered the Parent Category by Theater within the pivot table to analyze the theater category.
The line graph shows the number of completed, failed, or canceled projects by month. We can see how each month influenced the fundraising campaign outcome using the line chart visualization.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/105666905/174185738-02cbb236-c6f4-4caf-a6e2-a81c74bc50f8.png)

May is the month with the most successful Kickstarter campaigns, we can conclude. However, the number of failed campaigns was roughly the same in May, June, July, August, and October.

### Analysis of Outcomes Based on Goals

I crafted another line chart based on the funding goal amounts to show the percentage of successful, failed, and canceled plays.
First, I made a sheet titled "Outcomes Based on Goals" with the columns listed below:

Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, Percentage Canceled.

Then, within the "Goals" column, I organized the projects by the dollar amounts listed below:

Less Than $1000, $1000-$4999, $5000-$9999, $10000-$14999, $15000-$19999, $20000-$24999, $25000-$29999, $30000-$34999, $35000-$39999, $40000-$44999, $45000-$49999, Greater than $50000

I then used the COUNTIFS() function to collect the outcome and goal data from the "plays" subcategory to populate the number of successful, failed, and canceled projects. For example, to count the number of successful plays with a goal of less than 1000, I used the following function: =COUNTIFS (Kickstarter!D:D, "1000," Kickstarter!F:F, "=successful," Kickstarter!R:R, "=plays")

At last, I made a line chart to show the relationship between the goal-amount ranges on the x-axis and the percentage of successful, failed, and canceled projects on the y-axis.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/105666905/174196667-2b5dffcf-8c31-4059-8607-54929a7eb122.png)

We can deduce that there is a link between the campaign's success or failure rate and the goal amount. As the funding goal amount increases, we can deduce that the rate of successful projects will decrease. However, a few projects with budgets ranging from $35,000 to $34,999 and $40,0000 to $44,999 were successfully launched. Because of the dataset's limitations, the reason for the discrepancy is unknown. We could theorize that the projects with higher goals had higher demand and a better marketing campaign to generate more interest, but our current dataset does not support this. More data sets would help us apply this theory and gain a better understanding of it.

### Challenges and Difficulties Encountered

It's difficult to explain why budgets in the higher range resulted in more successful projects. The total number of projects in the dataset is one of its constraints. As a result, we can only presume as to why this range had a higher number of successful campaigns due to various factors that were not included in the dataset.

## Results

Based on our data, we know that the best time to launch a campaign is in May. The end of the summer months still appears to have a high failure rate, making it a high-risk, high-reward season.

We can conclude with certainty that the majority of these high-budget forced campaigns were failures. We know that films with a lower budget have the most success, while those with a higher budget have a higher rate of failure. We can't just force a play with money. Some, however, were successful in the $35,000-$45,000 range, so we'd benefit from more data.

Additional tables and graphs can be generated to further analyze the Kickstarter campaigns. It would be beneficial to conduct a comparative analysis of theater campaigns in relation to the other 8 parent categories.
