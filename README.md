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
