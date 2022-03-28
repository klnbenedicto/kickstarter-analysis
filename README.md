# Kickstarting with Excel

## Overview of Project

### Purpose - After getting close to reaching her fundraising goal, Louise wants to know how the launch dates and funding goals impacted the outcome of other campaigns. The purpose of this assignment is to visualize outcomes based on their launch date and outcomes based on their goals.

## Analysis and Challenges

![Outcomes Based on Launch Date](/assets/images/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Launch Date - Theater Outcomes by Launch Date is a visual representation of the success, failure, and cancelation of theater campaigns based on the month the campaign went live. To get this chart, I created a pivot table with filters for Year and Parent Category and then filtered for theater campaigns. The columns were set to Outcomes, rows to Date Created, and the values of the table are the Outcome of Campaign. Once I had a pivot table, I created a line graph and added a chart title and axis labels.

![Outcomes Based on Goals](/assets/images/Outcomes_vs_Goals.png)

### Analysis of Outcomes Based on Goals - Outcomes Based on Goals is a visual representation of the percentage of successful, failed, and canceled campaigns based on their goal. I used COUNTIFS() to get the number of outcomes for each range of goals and then used SUM() to get the total for each range. From there, I created three new columns to calculate the percentages and divided the number of each outcome by the total number of projects. I made a line graph out of the percentages, added a chart title, and labeled the x-axis.

### Challenges and Difficulties Encountered - I didn't face any challenges with Deliverable 1, but a potential challenge I could see would be getting the Date Created raw data converted to an actual date for the Theater Outcomes by Launch Date. Luckily, I had the module exercises to walk me through that. For Deliverable 2, I was getting inaccurate counts for goals that were a range rather than "less than $1,000" and "$50,000 or more". I realized I was only including the top number of the range and saying it had to be less than that. I corrected the formula to include greater than or equal to the bottom of the range and was able to get accurate readings from there. I also thought I had input the wrong formula for Number Canceled, since they were all zeros, but I went back to the raw Kickstarter data, filtered for "plays" and checked - there were no canceled campaigns.

## Results

Theater Outcomes by Launch Date shows that the best month to launch a theater campaign is May. May has the highest number of total theater campaigns launched, the highest number of successful campaigns in this category, and the highest percentage of successful campaigns to the total at 67%. The worst month to launch a theater campaign is December. December has the lowest count of successful campaigns and highest percentage of failed campaigns at 47%. 

Play Outcomes Based on Goal shows that the percentage of success with for play campaigns was highest when the goals were under $5,000. Additionally, there was a high percentage of success for goals between $35,000-$45,999, but total number of projects in that range was lower. The range with highest percentage of failed campaigns was $45,000-$49,999. 

The data is only quantitative, not qualitative. There could be other factors that contribute to the success or failure of each campaign such as quality of the concept. Another limitation with the analyses of this dataset is that the results could be telling a story due to quantity in certain ranges. For example, Outcomes based on Goals had 100% of campaigns fail, so there is a large spike in the chart. However, there was only one campaign, so in this case, the data doesn't feel as significant as the chart makes it look.

It would be good to further tell the story if we visualized the distributions with a Box Plots of Successful next to Failed play outcomes with the range showing the goal amount. 