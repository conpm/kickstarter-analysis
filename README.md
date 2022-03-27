# kickstarter-analysis
---
# Analysis of Kickstarter Theater Campaigns
## Overview of Project

### Purpose
The purpose of this analysis was to demonstrate the relationships between Kickstarter campaign outcomes and their launch dates as well as their funding goals.  The analysis was performed in order to show trends in these relationships within Kickstarter data specifically related to projects in the category of theater and the subcategory of plays.  This was done in order to help a client, Louise, in order to better understand how her Kickstarter campaign to fund her play "Fever" can succeed.   
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The analysis was started by creating some additional collumns in order to further filter the data.  The collumns which were created were for parent category and subcategory.  Additionally, the launch dates and deadlines were converted from Unix time stamp into Month/Day/Year format in order to make them more easily understandable, and this converted date was additionally split into an additional collumn just displaying the year in order to further filter the data.  Then by utilizing these additional collumns as filters, I was able to create this line chart which demonstrates the relationship between the outcomes of Kickstarter campaigns within the theater parent category and when they were launched.
![Theater Outcomes vs Launch](https://github.com/conpm/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)
### Analysis of Outcomes Based on Goals
Next, the data was filtered using a variety of ranges of Kickstarter goals as well as with the subcategory of plays.  Ther ranges were set starting with goals below $1000 and ending with Goals greater than or equal to $50000, between these two ranges the data was split into 10 additional ranges of approximately $5000 each.  Utilizing these filters, a count of projects with each outcome (successful, failed, and canceled) was calculated for each goal range.  Those counts were further broken down to show a percentage of the total projects within the range which resulted in each outcome.  Using this filtered dataset, I created this chart which shows the relationship between the outcomes of Kickstarter campaigns within the play subcategory and their intial fundraising goals.
![Outcomes vs Goals](https://github.com/conpm/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)
### Challenges and Difficulties Encountered
During the course of the analysis there were two challenges that I encountered in order to make the data legible and accurate.  The first challenge I encountered was getting the row labels to display only the month within the pivot table created for the Theater Outcomes vs Launch chart.  In order to solve this I had to group the date created collumn so that it only counted by month.  The second challenge that I encountered was getting my data to display as percentages in the pivot table used to create the Outcome vs Goals chart.  The reason I encountered this problem was due to correcting the calculation for percentage into a whole number by multiplying the function by 100.  I was able to solve this by keeping the percentages in a decimal format and then utilizing the number formatting in excel to display those numbers as percentages instead of General numbers.
## Results

- Conclusions based on Theater Outcomes vs Launch
  - The first noticable conclusion that can be drawn from the Theater Outcomes vs Launch chart is that Kickstarter campaigns within the Theater parent category are most likely to succeed when they are launched in the spring/summer season, with the highest level of success coming from campaigns launched in May.
  - The second conclusion that can be drawn is that Kickstarter campaigns are less likely to succeed when they are launched in the fall/winter season, with the lowest number of successful campaigns launching in December, as well as the highest number of failed campaigns launching in October.
- Conclusions based on Outcomes vs Goals
  - From the Outcomes vs Goals chart it can be concluded that Kickstarter campaigns within the plays subcategory are most likely to succeed when their goals are less than $5000.  
  - Additionally it shows that campaigns with goals between $20000 and $34999 as well as campaigns with goals over $45000 are much more likely to fail.
- Limitations of the dataset
  - The limitations of this dataset are primarily surrounding the scope of the data, specifically that the data only represents approximately 1400 Kickstarter campaigns in the Theater parent category and only 1000 of which being in the plays subcategory.
  - Additionally, the dataset only convers from the year 2009 to the year 2017 and by leaving out data from the past 5 years it is possible that new emerging trends could change some of our conclusions.
  - Finally, this dataset only shows success as a measure of whether or not the Kickstarter campaign acheived their funding goal or not.  While this does demonstrate the success of the campaign it does not take into consideration how any of the project performed after achieving their goals.  Therefore it could be possible to have campaigns which successfully acheived their funding goal but did not have success after the goal was reached.
- Possible additional tables and/or graphs
  - A graph showing outcomes in relation to average donation amounts in order to set appropriate donation amounts within the campaign.
  - A graph showing outcomes in relation to whether a campaign was a staff pick and/or was featured in the spotlight section of the website could show how these features of the kickstarter platform can contribute to campaign success.
