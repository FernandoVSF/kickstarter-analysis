# Kickstarting with Excel

## Overview of Project

### Analyze how different campaigns fare in relation to their launch dates and funding goals

## Analysis and Challenges

### The analysis of outcome based on launch date was performed creating a Pivot Table filtering data by parent group and years, having the outcomes as columns and date created grouped by months as rows.  Then a Pivot Chart was created to analyze the trend.  
 
### The analysis of outcome based on goal was performed creating a worksheet using range of goals as rows and outcomes as columns. Then, using conditional counting (countifs), data was filtered to show only subcategory plays, breaking data into ranges and outcomes.  Finally, the percentage was calculated per each range/outcome, and a line chart was created to analyze trends

### Some challenges and difficulties were encountered in the process.  On the outcome based on goal, there were too many hardcodes in the formulas, which makes it difficult to change parameters and debug errors.  The solution was creating outside cells with lower and upper bound of the range, the outcomes and subcategory, so there is no hardcoding in formulas. 

## Results

- Through the analysis on the outcomes based on launch date we can draw 2 conclusions:

1.	Best month to launch a campaign is May;
2.	Worst month to launch a campaign is December.

-	However, the analysis is a bit biased, since May is the month most of the campaigns start, and December is the least of them.  It is hard to infer a cause consequence effect, as the reason for more launches can be because they are more successful in average.   To validate the data, I calculated the success as percentage of total, and still got May as the best and December as the worst, but with less dispersion from average.

- Through the analysis on the outcomes based on goals, we can conclude that the higher the goas are set, it decreases the success ratio

- This database presents some limitations, as follows:
	- Goals can be attributed without much criteria, with some of them been unrealistic target
	- Presence of couple of outliers
	- High Standard Deviation in Goals and Pledged, even if we consider only successful campaigns

- Other possible tables/graphs we could create are:
	- For Outcomes based on Launch Date we could create a table/chart or success ratio (success over total excluding live)
	- For outcomes based on goals we could use a Pivot Table filtering by subcategory plays, using outcome as columns and goals as rows grouped in range of 5000.  We could also make a regression of goals against percentage of success and fails.
