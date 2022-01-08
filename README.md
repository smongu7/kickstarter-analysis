# An Analysis of Kickstarter Campaigns
## Overview of Project
The purpose of this project was to become familiar with many functions of Excel-- especially creating pivot charts. To accomplish this, we were given an example scenario: An individual-- Louise-- wants to kickstart a campaign for a play she wants to produce. Before beginning, she wants an analysis of several kickstarter campaigns. Using the data set she gives us, we create multiple pivot tables and pivot charts to identify and visualize trends seen in the data. Using the analyses performed, we are then able to draw conclusions about successful versus failed campaigns. To help illustrate and explain to Louise the conclusions we draw, we use the charts created to visualize the trends.
## Analysis and Challenges
I performed the analysis by first creating a pivot table of the data. I then filtered the data by (parent) category and year, followed by placing "outcomes" and "date created conversion" into columns and rows, respectively. I also placed outcomes under values, which then became "count of outcomes" The resulting pivot table looked something like this:

![pivot_table_1b](https://user-images.githubusercontent.com/94420548/148625728-b6207060-0417-475c-bc41-f4878de25953.png)

When creating the chart to see the outcomes based on launch date, I filtered the pivot table to display the information for the theater (parent) category, as shown here:

![Pivot_table_1c](https://user-images.githubusercontent.com/94420548/148625793-72ed4bd7-cc0f-43db-9aef-1d9d7c724c16.png)

This was the process used to analyze the data for outcomes based on launch date.

Analyzing the data for outcomes based on fundraising goals began a little differently. I created a new sheet with 12 different goal categories listed in ascending order. For each goal category, I calculated the number of successful, failed and canceled projects using the COUNTIFS function. I then calculated the percentage of successful, failed and canceled projects to get a table that looked like this:

![screenshot_1](https://user-images.githubusercontent.com/94420548/148627409-4a868adb-a73a-4140-892c-5a7dee64c88d.png)

Then, using the percentage columns, I created a chart illustrating the percent of successful and failed outcomes based on goal.

The biggest challenge I encountered was figuring out how to use the the COUNTIFS formula. I had to be careful and  consistent about where I put the quotation marks around the outcome, the subcategory, and the goal ranges. Additionally, I had to make sure I was placing the greater then versus the greater then *or equal to* symbols correctly. Once I figured out the first cell of COUNTIFS function, the rest were relatively easy; it was just a little time consuming.

## Results

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/94420548/148628074-e2ec90fc-22ba-4e26-b4e4-17383945596d.png)

Based on this graph, May has the highest number of successful outcomes. May also has the highest number of failed outcomes, but the difference between the number of successful and failed outcomes is also at its largest in May; this means that May has the highest percentage of successful theater outcomes. Thus, from looking at this graph, I would advise Louise to kickstart her campaign in May. Additionally, December not only has the lowest number of successful outcomes, but it is almost equal to the number of canceled outcomes, meaning that roughly 50% of campaigns were canceled. According to this percentage, a theater campaign had about a 50/50 chance of ebing successful; in simpler terms: a flip of the coin.  Based on the data we have, kickstarting a campaign in December would be a gamble, and I would advise Louise not to kickstart a campaign in December.

This being said, I would also advise Louise that time of year is not the only factor in determining the outcome of a campaign, and I strongly recommend looking at other factors, like the effect fundraising goals also have on outcomes.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/94420548/148628116-1a9d28ce-5498-42e9-be80-716cd1b373a8.png)

Based on this graph, I can conclude that campaigns with a goal of less than $1000 have the highest chance of being successful. I would advise Louise to keep her campaign under $1000. Based on both graphs, I would advise Louise to kickstart her campaign in May with a goal of less than $1000. That said, these are only two factors affecting theater outcomes. More data that would be helpful would be theater outcomes based on launch date of several consecutive years. This way, we could see if the trend follows a similar pattern year to year. If we saw that, then we could conclude that launch date has a significant impact on outcome. This is probably the biggest limit to the data set-- we only have information for one year. I'd also recommend making graphs displaying the following: 
- outcomes based on category
- outcomes based on backers
- outcomes based on country and category

I would use the first of these graphs to see what category tends  to be the most successful. I would use the second to see if successful campaigns tend to have a certain number or range of backers. The third, I would use to see if certain categories do better in different countries. For example, let's say Louise wants to kickstart her campaign in the US. We could use the "outcomes based on country and category" graph to see what category of campaign tends to enjoy the most success in the US. Let's say that film & television saw the most success of all the categories in the US. I would then adivse Louise to kickstart her campaign for a film or television. If Louise cared more about her campaign being theater, and theater did best in Great Britain, I would advise Louise to kickstart her campaign in Great Britain.
