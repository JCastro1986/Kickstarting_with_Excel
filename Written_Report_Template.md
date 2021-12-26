# Kickstarting with Excel
Callenge #1. Create an analysis to help Louis understand how campaigns are going based on their launch dates and their fundings goals.
## Overview of Project
This project is to help Louis understand how campaigns are going based on their launch dates and their fundings goals.
### Purpose
Using the current data we have created we need to create a visualization from campaigns outcome based on launch dates and funding goals.
## Analysis and Challenges
I filter and clean the data provided by Louis that contain important information about her campaigns. The information contained information such as:
- Name of the campaign.
- Goal.
- Pledged.
- Outcome.
- Country.
- Launched date.
- Subcategory.
Based on such date, I need to create many columns that will facilitate my analysis, among the columns I created are the following:
- Percentage funded.
- Date created conversion.
- Date ended conversion.
- Years.
- Date created conversion (month)
### Analysis of Outcomes Based on Launch Date
Taking into consideration all the data I started by creating a PivoTable, thin in order to better visualize the data I wanted to see. I began by filtering by Parent category and Years, using the outcome in the columns section and having dates created in the raws section and count of outcomes in the values field. In order to better visualize the data, I proceeded to create a line graph that helped me view how successful, failed, and canceled campaigns have been responding based on the launch date. *This helped me see that the month with the most successful campaigns was May.*
### Analysis of Outcomes Based on Goals
After that I created tabular data using new columns that were populated using 12 goals criteria, starting from less than 1000 and going all the way up to greater than 50000. This was the real challenge for me because we used **COUNTIFS** function, I had used this function before but never as I did in this exercise. In order to better visualize the data, I created a line graph using the different goal criteria and the % of successful, failed, and canceled campaigns. *This helped me see that the best percentage of successful campaigns 76% had a goal of less than 1000, as well I noticed that as the goal went up the same did the percentage of failed campaigns.* 
### Challenges and Difficulties Encountered
 Doing the first and last goal criteria with COUNTIFS was easy, but the ones in the middle such as "1000 to 4999, 5000 to 99999..." were challenging. With this exercise, I learned that numeric criteria need to be added into the formula with "", and in order to have the more than and less than I need to add second criteria because they can't be just like this: ">=1000<=4999", rather: ">=1000","<=4999").
## Results
- What are two conclusions you can draw about the Outcomes based on Launch Date?
Based on my analysis I confirm that there is a higher tendency of having more successful campaigns when the launch date is May. 
Launching a campaign at the beginning of the year from January to April and at the end of the year from September to December will not be beneficial since data indicates those are the months with less successful campaigns.
The best months to launch a campaign will be May, June, and July, having the month of May as the best option for launching a campaign.
- What can you conclude about the Outcomes based on Goals?
Based on my analysis I confirm that there is a higher tendency of having more successful campaigns when the goal is less than 1000.
Having a campaign with a goal greater than 45000 is pretty much destined to fail. As well having a goal between 25000 and 35000 has shown a great percentage of failure. As well date confirms that the lowest percentage of failed campaigns is when the goal is less than 1000.
The best way to predict a successful campaign will be to have a goal that is less than 1000.
- What are some limitations of this dataset?
The main limitation is that I am working with a sample based on Louis data, I do not have all the population of campaigns available for my analysis.
- What are some other possible tables and/or graphs that we could create?
I could have created a Box and Whisker graph to identify and address outliers.
I could have added measures of central tendency to base my analysis on calculations and confirm if our data is skewed to the right or to the left or if our data is symmetric. 