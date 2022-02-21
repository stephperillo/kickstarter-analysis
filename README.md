# Kickstarting with Excel

## Overview of Project
This project is an analysis of kickstarter data. 

### Purpose

The purpose of this project is to showcase the data from different kickstarter campaigns with the intent to reveal the factors that may have contributed to their success.

## Analysis and Challenges

Two areas of the data that I highlighted were the Outcomes based on Launch Date and Outcomes based on Goals. 

### Analysis of Outcomes Based on Launch Date

This selection of data compares the outcomes of theater kickstarters based on the month of each's respective launch date. I created a PivotTable and May and June are the two months in which the highest number of successful theater kickstarters were launched. The data shows that the failed and canceled numbers did not vary much with the launch month. The month of December proves to have the lowest number of successful theater kickstarters.

### Analysis of Outcomes Based on Goals

This analysis categorizes the kickstarters based on the goal amounts in order to show the differences in results. The percentages of successful, failed and canceled kickstarters were plotted against the varying goal amounts. The results align with the logic that if the goal amount is extremely high, such as $45,000 or more, there is a very low likelihood that the lofty goal will be reached. On the other hand, those with goals that were $35,000 to $44,999 were more successful that those with goals between $25,000 and $34,999.

### Challenges and Difficulties Encountered

One challenge that was encountered during this analysis was, when creating the Outcomes Based on Goals PivotTable, ensuring that the counts of kickstarters by goal were not only counting the data for the number of successful/failed/canceled kickstarters in each goal amount range, but also only counting the number within subcategory of plays specifically. 

For example: 

"=COUNTIFS(Kickstarter!D:D,">1000",Kickstarter!F:F,"successful",Kickstarter!R:R,"plays")" 
vs. 
"=COUNTIFS(Kickstarter!D:D,">1000",Kickstarter!F:F,"successful",Kickstarter!R:R)"

Failing to select for the number of successful kickstarters in the subcategory of plays yields a much lower result than all successful kickstarters. The same principle applies with the rest of the formulas for the counts in columns B, C, and D in that PivotTable. If the  erroneous table was plotted as a line graph, a vastly different line graph would be produced and that could have possibly been interpreted as the desired data, which would result in an inaccurate depiction of the data we are investigating. Learning from this challenge reveals that it is important to think about the data one is asking Excel to extract and use when using formulas to create tables, as well as recognizing when things don't look right or as expected based on what we already know.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The Outcomes based on Launch Date shows some important findings. Firstly, when looking at Theater Outcomes_vs_Launch.png: ![Theater_Outcomes_vs_Launch.png](https://github.com/stephperillo/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png) The line graph shows that the outcomes of theater kickstarters that launched in the months of May and June, despite the year, had a higher number of successful kickstarters compared to those with launch dates in other months, especially those that launched in the month of December. Another conclusion from this analysis is that the number of failed kickstarters remains relatively stable and has not ever dropped down below 31 or risen to over 52 per month. Overall, the number of successful theater kickstarters has always been greater than the number of failed and canceled theater kickstarters, which indicates that it would be worth a try to start a theater kickstarter. 

- What can you conclude about the Outcomes based on Goals?

The Outcomes based on Goals line graph: ![Outcomes_vs_Goals.png](https://github.com/stephperillo/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png) clearly shows that kickstarters with goals that were set to $45,000 or higher have failed at least 88 percent of the time, with those in the $45,000 to $49,000 goal range failing 100 percent of the time. If one is planning to start a new kickstarter for plays, it would be wise not to set the goal too high, since there is a high likelihood of failure. The goal range with the highest success rate relative to fail rate is $1000 to $4999, so setting the goal to an amount in this range may be best.  

- What are some limitations of this dataset?

While this dataset highlights interesting facts about theater kickstarters, this dataset has its limitations. A helpful sub level category of play genre or type, such as comedy or drama, could help reveal trends about the types of plays that have successful kickstarters so that theater professionals make more informed decisions about the type of play they may choose to begin producing and crowdfunding.

- What are some other possible tables and/or graphs that we could create?

It would be useful to create other tables and graphs with this dataset. One example of this would be a table and graph to show the differences in deadline duration to portray if the duration of the kickstarter tends to affect the success rate, and if so, how.  
