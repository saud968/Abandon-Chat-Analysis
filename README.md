# Abandon-Chat-Analysis
![Intro Image](https://github.com/saud968/Abandon-Chat-Analysis/blob/main/Intro%20Page.png)

## Introduction:
This is a Power BI project on the “Abandon Chat Analysis”. The
project is to analyze and derive insights into the abandon, total chat count and abandon percentage to make data-driven decisions.

## Problem statement:
1. What is the Abandon Count and Percentage in the current year and months?
2. What is Abandon Percent by day, hours, and months?
3. Which are the top products?
4. Which are the top business groups?

## Skills/concepts demonstrated:
The following Power BI features were incorporated:
-	Bookmarking, 
-	DAX, 
-	Measures, 
-	Page navigation, 
-	Filters, 
-	Conditional formatting for Background color for Heatmap,
-	New Button Slicers.

## Features:
1. The heatmap is to identify the abandon, total chat count and abandon % month-wise, day-wise, and hour-wise.
   ![Heatmap](https://github.com/saud968/Abandon-Chat-Analysis/blob/main/Heatmap%20Abandon%20%25.png)
2. Important Dax used to Sort the Days in Heatmap.
   - **1. Day Name_ = REPT(UNICHAR(8203),7-support__cw_ops_manage_case_merge_temp[WeekDaySort])& support__cw_ops_manage_case_merge_temp[DayText].**
   - **2. DayText = SWITCH(support__cw_ops_manage_case_merge_temp[WeekDaySort], 1, "Monday", 2, "Tuesday", 3, "Wednesday", 4, "Thursday", 5, "Friday", 6, "Saturday", 7, "Sunday", "Unknown").**
   - **3. WeekDaySort = SWITCH(support__cw_ops_manage_case_merge_temp[Day], "Monday", 1, "Tuesday", 2, "Wednesday", 3, "Thursday", 4, "Friday", 5, "Saturday", 6, "Sunday", 7, 8)****

## Visualization:
The report is set on multiple pages as per the requirement:
1.	Summary Page.
2.	Abandon Heatmap. 
3.	Pillar Abandon Heatmap.
4.	Raw Data.

## Analysis:

1. Summary Page.
![Summary Page](https://github.com/saud968/Abandon-Chat-Analysis/blob/main/Intro%20Page.png)
This page gives us abandon, total chat count, and abandon % month-wise, day-wise, and hour-wise with different visuals like Matrix, Bar and Line Chart, and Small Multiples. 
![Abandon Week by Hours](https://github.com/saud968/Abandon-Chat-Analysis/blob/main/Abandon%20by%20Week.png)
![Abandon Month by Hours](https://github.com/saud968/Abandon-Chat-Analysis/blob/main/Abandon%20by%20months%20by%20hours.png)
![Abandon Bar and Line Chart](https://github.com/saud968/Abandon-Chat-Analysis/blob/main/Abandon%20Overall%20Bar%20and%20Line%20Chart.png)
![Abandon Small Multiples](https://github.com/saud968/Abandon-Chat-Analysis/blob/main/Abandon%20Overall%20Bar%20and%20Line%20Chart%20(Small%20Multiples).png)

2. Abandon Heatmap.
![Abandon % Heatmap](https://github.com/saud968/Abandon-Chat-Analysis/blob/main/Heatmap%20Abandon%20%25.png)
![Abandon Total Count Heatmap](https://github.com/saud968/Abandon-Chat-Analysis/blob/main/Heatmap%20Total%20Chat%20Count.png)
![Abandon Count Heatmap](https://github.com/saud968/Abandon-Chat-Analysis/blob/main/Heatmap%20Abandon%20Count.png)
This page gives us abandon, total chat count, and abandon % month-wise, day-wise, and hour-wise in a heatmap version.

3. Pillar Abandon Heatmap.
![New Slicer Button](https://github.com/saud968/Abandon-Chat-Analysis/blob/main/New%20Button%20Slicer.png)
![Abandon % Heatmap](https://github.com/saud968/Abandon-Chat-Analysis/blob/main/Heatmap%20Abandon%20%25.png)
![Abandon Total Count Heatmap](https://github.com/saud968/Abandon-Chat-Analysis/blob/main/Heatmap%20Total%20Chat%20Count.png)
![Abandon Count Heatmap](https://github.com/saud968/Abandon-Chat-Analysis/blob/main/Heatmap%20Abandon%20Count.png)
This page gives us abandon, total chat count, and abandon % month-wise, day-wise, and hour-wise in a heatmap version. However, it has a new slicer button that allows to separate the business groups which is known as Pillar. 


