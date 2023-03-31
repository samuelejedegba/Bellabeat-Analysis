# Bellabeat-Analysis
![](https://github.com/samuelejedegba/Bellabeat-Analysis/blob/main/bellabeat.png)

## Introduction

Bellabeat is a successful small company which is a high-tech manufacturer of health-focused products for women, but they have the potential to become a larger player in the global Smart device market. The cofounder and Chief Creative Officer of Bellabeat, believes that analyzing smart device fitness data could help unlock new growth opportunities for the company. You have been asked to focus on one of Bellabeat’s products and analyze smart device data to gain insight into how consumers are using their smart devices. The insights you discover will then help guide marketing strategy for the company. You will present your analysis to the Bellabeat executive team along with your high-level recommendations for Bellabeat’s marketing strategy. Belabeat products include:
1. Bellabeat app: The Bellabeat app provides users with health data related to their activity, sleep, stress, menstrual cycle, and mindfulness habits. This data can help users better understand their current habits and make healthy decisions. The Bellabeat app connects to their line of smart wellness products. 
2. Leaf: Bellabeat’s classic wellness tracker can be worn as a bracelet, necklace, or clip. The Leaf tracker connects to the Bellabeat app to track activity, sleep, and stress. 
3. Time: This wellness watch combines the timeless look of a classic timepiece with smart technology to track user activity, sleep, and stress. The Time watch connects to the Bellabeat app to provide you with insights into your daily wellness. 
4. Spring: This is a water bottle that tracks daily water intake using smart technology to ensure that you are appropriately hydrated throughout the day. The Spring bottle connects to the Bellabeat app to track your hydration levels.
5. Bellabeat membership: Bellabeat also offers a subscription-based membership program for users. 
Membership gives users 24/7 access to fully personalized guidance on nutrition, activity, sleep, health and beauty, and mindfulness based on their lifestyle and goals.

## Problem statement

1. What are some trends in smart device usage? 
2. How could these trends apply to Bellabeat customers? 
3. How could these trends help influence Bellabeat marketing strategy? 

## Dataset
The dataset was acquired from [here](https://www.kaggle.com/datasets/arashnic/fitbit). I worked with all the  ‘Daily activity’ data sets to get a broader view of the data. This dataset contains information about 33 users of the Fitbit Fitness Tracker. Some of the data in this dataset include date, calories, Activities, Steps, Distance, Active minutes, Sleep and Weight. The data for sleep and weight have 22 and 8 unique entries instead of 33 like the others. This calls into question the integrity of the data.

## Skills/Concepts demonstrated
1.	SQL
2.	Power BI

## Cleaning and Analysis
For the cleaning, I used SQL for cleaning and manipulation of data. I created smaller tables with new information in order to make more sense of the data.

![](https://github.com/samuelejedegba/Bellabeat-Analysis/blob/main/SQL%20analysis%201.PNG)
![](https://github.com/samuelejedegba/Bellabeat-Analysis/blob/main/SQL_analysis%202.PNG)

Step 1 – I created a table with ID, total steps, total distance and total calories using ‘Sum’ functions and ‘Group by’ statement.

Step 2 – I created a table with ID, weekday and the different classifications of activity which is grouped into Active minutes, Fairly active minutes, lightly active minutes and sedentary minutes, using ‘datename’ function to get the day of the week, sum function and ‘Group by’ statements.

Step 3 – I created a table with weekday, Total Minutes Asleep and Total Time in bed using the ‘datename’ function and ‘Group by’ statement.

Step 4 – Split the date and the time column into date and time using the ‘charindex’ function.

Step 5 – Exported the data into Power BI for analysis.

## Visualization
![](https://github.com/samuelejedegba/Bellabeat-Analysis/blob/main/Total_steps_and_calories.PNG)

The above chart shows the relationship between steps and calories and shows that the more the steps these users take, the more calories they burn.
![](https://github.com/samuelejedegba/Bellabeat-Analysis/blob/main/sum_of_steps_per_weekday.PNG)

The above chart shows the number of steps by day of the week. It shows that the users take the least steps on a Sunday but are most active on Tuesday.
![](https://github.com/samuelejedegba/Bellabeat-Analysis/blob/main/total_share_of_activity.PNG)

The above chart shows the activity share. The sedentary active minutes makes up a huge 81.33% of the total activity by these users. Active minutes makes up only 1.74% of the activity minutes.
![](https://github.com/samuelejedegba/Bellabeat-Analysis/blob/main/Activity_per_weekday.PNG)

The above chart shows the share of activity but this time by weekday and it tells the same story. Sedentary minutes take the largest share of the active minutes especially on Tuesday.
![](https://github.com/samuelejedegba/Bellabeat-Analysis/blob/main/Activity_by_time.PNG)

The above chart shows the Intensity by time of the day. Intensity picks at 6PM.

Conclusions and Recommendations
1.	Bellabeat creates health focused products for women. Creating a reward system for the number of steps taken which leads to losing more calories would encourage users to take more steps and get more active.
2.	The leaf/Time can track the sedentary minutes and alert the user then it is getting too much, encouraging them to be more active.
3.	Bellabeat application can create a weekend challenge with points and reward to encourage more activity in the weekend, especially Sundays.
