# Kickstarting with Excel

## Overview of Project
### Purpose
Louise, an up-and-coming playwright, is wanting to do a crowdfunding campaign that will help her fund her play “Fever”. Louise figures “Fever” has a budget of around $10,000. She is hesitant to jump into her first ever fundraising program and is seeking help from an excel power-user on organizing, sorting, and analyzing crowdfunding data. The help Louise is needing is to help in determining if there are specific factors that will make a project campaign be successful. By using excel to analyze the data, Louise will get a better understanding of campaigns from start to finish and help her set her campaign to mirror other campaigns in the same category that were successful.

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
An analysis was done on "Theater Outcomes Based on Launch Date" by creating a pivot table that shows how many campaigns for theaters/plays were successful, failed, or canceled. The fields that were used for the pivot table was “Outcomes”, “Parent Category” (theater), and “Date created conversion”. The “Date created conversion” field is what allowed the outcomes to be broken down by years and months. A line chart was created to show more of the picture of the successful, failed, and canceled campaigns.
![Theater_Outcomes_vs_Goals](https://github.com/fletchrk/kickstart-analysis/blob/main/Resources/Theater_Outcomes_vs_launch.png)

### Analysis of Outcomes Based on Goals
An analysis based performed on “Outcomes Based on Goal” was performed by creating a table using COUNTIFS() and SUM() functions in excel. The columns that were used were the outcome, goal, and the sub-category columns. The COUNTIFS() function was used to determine which plays had outcomes of successful, failed, or canceled depending on their goal amount. The SUM () function was used to determine the total number of projects that were successful, failed or canceled depending on the plays goal. Percentages of successful, failed, and canceled projects were each calculated by each the goal range row. 
![Outcomes_vs_Goals](https://github.com/fletchrk/kickstart-analysis/tree/main/Resources)

### Challenges and Difficulties Encountered
There were no challenges that occurred while performing the analysis. Some challenges that could have occurred is that Excel has no control of errors so that makes them error prone. What I mean by this is that excel does not have any tools that will help inspect that all cells are working as expected especially after a change. Excel is great for simple and ad hoc calculations, but it is lacking structure and has a difficult time in automating and documenting contents to make sure excels use is error prone. Another challenge is Excel is not user-friendly. For example, macros are not easy to code/debug and  when it comes to multiple formulas there is not an easy overview of the dependencies between each other unless complex VBA code is used.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
The conclusions that were determined from the analysis on the "Theater Outcomes Based on Launch Date" was that there was a grand total of 1,369 campaigns done during the years of 2009-2017. Of those 1,369 campaigns, the data shows that 839 campaigns were successful (61%), 493 were failed (36%), and 37 were canceled (3%). The analysis shows that the month with the highest success was in May (111), while the month with the least successful campaigns was December (37). May also has the highest number of failed campaigns (52) and November has the least number of failed campaigns (31). 

- What can you conclude about the Outcomes based on Goals?
The conclusion that was determined on the “Outcomes Based on Goal” analysis is that of the 1047 plays that were analysed that 694 (66%) plays were successful at reaching their goal, 353 (34%) plays failed at reaching their goals. The highest number of plays (388) that were successful was in the goal range of 1000 to 4999 while no plays were successful at the goal range of 45000 to 49999. The highest number of plays (146) to fail was in the goal range of 1000 to 4999. The analysis shows that there were no plays that canceled at the goal ranges used. Another outcome that was determined is that the average percentage of plays that were successful was 45% and the average percentage of plays that failed was 55%

- What are some limitations of this dataset?
A limitation to the data set was that the category and subcategory was not broken down enough, so two new columns were created (Parent category and Subcategory) to better break down the categories. Another limitation is that the deadline date (Column I) and launched at date (Column J) was UNIX timeline, so a new column had to be created to convert the time to an actual date. 

- What are some other possible tables and/or graphs that we could create?
A chart/table that may be helpful is to do similar analysis as "Theater Outcomes Based on Launch Date" and “Outcomes Based on Goal” by country where the plays are originated out of. I think by figuring out which country is better at reaching goals and being successful, failed, or canceled would give Louise some guidance on how each country does crowdfunding campaigns.
