# Kickstarting with Excel

## Overview of Project
	After a successful kickstarter campaign, Louise wanted to see how similar campaigns did based on their launch date an their goal amount. 

### Purpose
	Help Louise see the outcomes of other play kickstarters based on their launch date and their goal amount, to perhaps inform future kickstarters on her own, or identify what she could have done differently. 

## Analysis and Challenges
	Started off with a diverse data set of kickstarters. Then, focused only on parent category "theater" and for one of the charts not the subcategory "plays". Looked specifically at the goal money amount and launch date to see if any of these would impact the success of a kickstarter campaign. 

### Analysis of Outcomes Based on Launch Date

	 I located the kickstarter tab and inserted a pivot table on a new sheet. I added the parent category and years to filters section. I then selected the "Date Created Conversion" for the rows section. I had to remove the quarters and years that generated automatically. I dragged the outcomes to the columns section and the values section, to see the number of succeeded, failed, or canceled kickstarters. I then filtered "theater" as the parent category. I also filtered the column labels to not include "live". Then, I sorter the the column labels descending. 

![](screenshots/image_1.png)

The final step was to create a line chart to look for trends. To do this, I first inserted a pivot chart. Then, I right clicked to change the chart type, and selected "line with markers'.

### Analysis of Outcomes Based on Goals
	I first crated a new sheet, and titled the first column "Goal". I then created subcategories of goal amounts in each row. In the following columns, I showed the number of successful, failed, and canceled play kickstarters for each goal amount. To do this, I  used the "count if" function to only add up only specified outcomes and goal amounts in the plays subcategory. I then calculated the outcome percentages by diving the number of one outcome by the total outcomes in that goal amount. To have the number show up as a percentage, I changed the number format to percentage for the applicable columns.

![](screenshots/image_2.png)

I then inserted a pivot chart and dragged the "goal" to rows, and the percentage successful, percentage failed, and percentage canceled to the values section. Once I had this, I inserted a line chart to visualize the data. 

![](screenshots/image_3.png)

### Challenges and Difficulties Encountered
A challenge I encountered with the Outcomes Based on Goal Chart was ordering the goal amounts in the right order. Doing a simple ascend or descend sort would not get them in the desired order. So what I did was I moved individual row labels to the up or down as needed by right clicking on the label, selecting move, and then choosing whether to go up or down. This allowed me to get the table to look a way that would make sense for the reader.  

![](screenshots/image_4.png)

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date? 

![](resources/Theather_Outcomes_vs_Launch.png)
	
If you only looked at failed kickstarters, it might seem that the number of failures increased May-August. However, when you look at the successful campaigns, you can see that those launches in May, June, and July saw the most success. Thus, the uptick in failures during those months is likely due to a higher number of kickstarters launching those months.

- What can you conclude about the Outcomes based on Goals?

![](resources/Outcomes_vs_Goals.png)

	In general, the smaller the goal for the kickstarter, the more likely the campaign was to succeed. 

- What are some limitations of this dataset?
	The "Outcomes Based On Goal" data was using money amounts that spanned different currencies and countries. Standardizing to one currency or looking at just one country at a time might help paint a better picture of what can be expected. However, that would decrease the volume of data. The more data available, the more confident you can feel about the conclusions drawn from it. 

- What are some other possible tables and/or graphs that we could create?

	We could look at US only plays and see recreate an "Outcomes Based on Goals" graph to see if the country affects the kickstarter success.

