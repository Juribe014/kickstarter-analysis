# Kickstarter-Analysis
Performing analysis on Kickstarter data to uncover trends

# Written Analysis of the Results

## Overview of the project

The purpose of this analysis is to identyfy trends at different levels of a category and parameters. The initial analysis focuses on the launch date of theater outcomes. The second analysis focuses on the monetary goal bracket outcomes of plays. 

## Analysis and Challenges

### Theater Outcomes by Launch Date
For the Theater Outcomes by Launch Date analysis, the tools used were the YEAR() function, a pivot table and a line chart. This was a simple analysis, as the function only required one input. The pivot table automated the filtering and calculation processes. The line chart can be quickly filtered and updated as it is connected to a pivot table. It's simple to show all the years associated with each month as one can focus on a single year of the data set through the filters. The only challenge that I can envision, is understanding if there is a correlation between launch date and its outcome. That would require further analysis. 

### Outcomes Based on Goals
For the Outcomes Based on Goals, the tools used were the COUNTSIFS() function, the SUM() function and a line chart. This analysis was complicated by a couple of factors. The first factor was the COUNTSIF() function, as it required multiple inputs and the inputs changed depending on the goal monetary bracket. In smaller monetary brackets or in more monetary brackets this could become more time consuming. One way to automate this would be to seperate the brackets in the goal column into two columns or to use an extraction function. That way the COUNTSIFS() fuction would call a specific cell as opposed to hardcoding it. A nested IF() function might also be required for cases where only one parameter is required as it was for for the first and last cell. The way the data is rounded would require more decimal places, as the sum of the Percentage Successful and Percentage Failed is more than 100% for the 50000 or More comparison.  

## Results

### Theater Outcomes by Launch Date
From the gathered data it can be concluded that more Kickstarters were sucessful for Theater than they were failures or canceled. It can also be concluded that, May had the most successful Kickstarters. On the other hand Novemeber and December had the worst results for launched Kickstarters. 
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/104809098/168499665-328a6c3c-2fb5-44e2-ac0d-88bfaef62793.png)

### Outcomes Based on Goals
It can be determined that plays with monetary goals below 15000 to 19999, with a resurgance at 35000 to 44999 had the highest probability of success. It can also be determined that there were no cancelations under the subcategory of plays. 
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/104809098/168499657-18b5d911-783d-4c92-b142-29c1606f31be.png)

### Limitations of the Data Set

This data set has multiple limitations. For one is that one can't make a concrete conclusions as to what made one kickstarter successful and the other a failure. There are multiple points that are not shown in the database that can influence the outcomes. For one is the experince of the people incharge of the project, another is how the project was advertise. More information is required to understand how to launch a successful Kickstarter. As of right now, we can only make general conclusions that for some reason the probability of success might be better in May or with less monetary capital as the goal. 

### Possible Tables or Graphs
If more analysis is required for this categories, than a comparison of monetary goals vs launch date could be appropiate. It would also be necessary to understand what role the time difference between the launch date vs the deadline played into the success of the Kicksarters. For these comparisons a bar graph might be more appropiate.
