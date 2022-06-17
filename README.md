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
Less Than 1000, 1000-4999, 5000-9999, 10000-14999, 15000-19999, 20000-24999, 25000-29999, 30000-34999, 35000-39999, 40000-44999, 45000-49999, Greater than 50000

I then used the COUNTIFS() function to collect the outcome and goal data from the "plays" subcategory to populate the number of successful, failed, and canceled projects. For example, to count the number of successful plays with a goal of less than 1000, I used the following function: =COUNTIFS (Kickstarter!D:D, "1000," Kickstarter!F:F, "=successful," Kickstarter!R:R, "=plays")

At last, I made a line chart to show the relationship between the goal-amount ranges on the x-axis and the percentage of successful, failed, and canceled projects on the y-axis.
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/105666905/174196667-2b5dffcf-8c31-4059-8607-54929a7eb122.png)

We can deduce that there is a link between the campaign's success or failure rate and the goal amount. As the funding goal amount increases, we can deduce that the rate of successful projects will decrease. However, a few projects with budgets ranging from $35,000 to $34,999 and $40,0000 to $44,999 were successfully launched. Because of the dataset's limitations, the reason for the discrepancy is unknown. We could speculate that the projects with higher goals had higher demand and a better marketing campaign to generate more interest, but our current dataset does not support this. More data sets would help us apply this theory and gain a better understanding of it.
