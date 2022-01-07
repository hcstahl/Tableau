# Tableau 
https://public.tableau.com/app/profile/hcstahl
# Table of Contents
[Gantt Chart](#Gantt-Chart)</br>
[Population Pyramid](#Population-Pyramid)</br>
[Small Multiple Lines Chart](#Small-Multiple-Lines-Chart)</br>
[Bar Chart with KPI indicator](#Bar-Chart-with-KPI-indicator)</br>
[Dynamic Chart](#Dynamic-Chart)</br>
[References](#References)</br>


# Gantt Chart
For this chart I measured the length of time between two dates using a Gantt Chart.</br>
1. The time measurment is in the column field</br>
2. The category that is being measured is in the row field.</br>
3. The size card is a calculated field that measures the difference between the start variable and end variable.</br>
(This makes the length of the bars match the time difference)</br>
4.The field uses the DATEDIFF function.</br>
5.This field is also in the text card to display the length of time to the user.</br>
6.There is a calculated field for a date difference of 0 to have a different color for items that have no time difference.</br>

# Population Pyramid
The column fields holds two types of continious variables.</br>

1.The row field holds a discrete variable that is used to measure going down the chart.</br>
2.The type of chart is a bar, but the second column field is reversed to create the population pyramid look.</br>
3.To do this, right click the axis area and undernath the Scale header click reverse.</br>
4.The parameter is linked to the row field so the user can control the difference in years that is shown.</br>

# Small Multiple Lines Chart


# Bar Chart with KPI indicator
This includes an Arrow on the bar chart indicating by color whether a performance target was met or not.</br>
In this example the Arrow turns Red, and the amount dissapers if it fails to meet the target.</br>

1. Create a calculated field (Axis) that includes MIN (0.0)</br>
2. Put the Axis field as a second column field.</br>
3. Make the Axis field a shape type.</br>
4. Create a calculated field to determine if the threshold is met or not, and put this field in the color mark.</br>
5. Create two calulated fields, for above or under the threshold.</br>
6. Put the two fields in the label mark so you can display the amount inside the bars.</br>
7. Make the column fields into dual axis and synchronize the axis.</br>

# Dynamic Chart
For this example I chose not to use icons, and just display the options using a normal parameter.</br>
1. Going to make the chart type for each option on a different sheet.</br>
2. Create a parameter string and put each chart name option in a list.</br>
3. Create a calculated field that returns the chart the user selects. The field only contains the parameter you just made.</br>
4. Drag this calculated field in the filter section for each chart and check the chart option that pops up.</br>
Putting into a dashboard:</br>
1. Put each chart inside a container and hide the titles for each container</br>
# References 
[Gantt Chart]()</br>
[Population Pyramid](https://playfairdata.com/how-to-make-a-diverging-bar-chart-in-tableau/)</br>
[Small Multiple Lines Chart](https://www.youtube.com/watch?v=kWZoa3UfbVs)</br>
[Bar Chart with KPI indicator](https://www.youtube.com/watch?v=e8yQGdKG6dI)</br>
[Dynamic Chart](https://www.youtube.com/watch?v=yEApDIou2hg)</br>
