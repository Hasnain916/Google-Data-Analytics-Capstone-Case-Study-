# Google Data Analytics Capstone: Cyclistic Case Study
Course: [Google Data Analytics Capstone: Complete a Case Study](https://www.coursera.org/learn/google-data-analytics-capstone)
## Introduction
In this case study, I will perform many real-world tasks of a junior data analyst at a fictional company, Cyclistic. To answer the key business questions, I will follow the steps of the data analysis process: 
Ask 
Prepare 
Process 
Analyze
Share

## Background
Cyclistic, a bike-share program in Chicago, offers diverse bicycles and docking stations, aiming for inclusivity.
Marketing shift: Convert casual riders to annual members for sustained profitability and growth.
Ask
Business Task: Devise marketing strategies to convert casual riders to members.

## Prepare
Data Source: Cyclistic’s historical trip data from Jan 2022 to Dec 2022.
Data Organization: 12 files (GYM-divvy-trip data) with essential ride details.
## Process
Data Handling: Used BigQuery for scalability, combining 12 files into '2022_tripdata'.
Data Exploration: Explored missing values, duplicates, and unique bike types.
Data Cleaning: Removed null values, excluded extreme trip durations, and refined columns.
## Analyze and Share
Data Analysis: Explored bike usage patterns by members and casual riders.
Visualizations: Created visualizations in Tableau for clear insights.
## Key Findings
59.7% members vs. 40.3% casual riders.
Member trips peak during commute hours; casual riders prefer weekends and daytime.
Casual riders take longer rides (2x) for recreation; members have consistently shorter rides.
Starting/ending stations: Casual - recreational spots; Members - universities, residential, and commercial areas.
Act
## Recommendations:
Conduct targeted campaigns at recreational spots in spring/summer.
Offer seasonal or weekend-only memberships.
Incentivize longer rides with discounts.
These insights can inform marketing strategies for Cyclistic's goal of converting casual riders into profitable annual members.

### Data Cleaning  
1. All the rows having missing values are deleted.  
2. 3 more columns ride_length for the duration of the trip, day_of_week, and month are added.  
3. Trips with a duration of less than a minute and longer than a day are excluded.
4. A total of 1,375,912 rows are removed in this step.
  
## Analyze and Share
The data is stored appropriately and is now prepared for analysis. I queried multiple relevant tables for the analysis and visualized them in Tableau.  
The analysis question is: How do annual members and casual riders use Cyclistic bikes differently?  

First of all, member and casual riders are compared by the type of bikes they are using.  

![image](https://user-images.githubusercontent.com/125132307/226692931-ecd2eb32-ffce-481a-b3c2-a6c3b4f3ceb7.png)
  
The members make 59.7% of the total while the remaining 40.3% constitute casual riders. Each bike-type chart shows a percentage of the total. The most used bike is a classic bike followed by the electric bike. Docked bikes are used the least by casual riders. 
  
Next the number of trips distributed by the months, days of the week, and hours of the day are examined.  
  
![image](https://user-images.githubusercontent.com/125132307/230122705-2f157258-e673-4fc5-bbed-88050b6aae68.png)
![image](https://user-images.githubusercontent.com/125132307/230122935-8d0889c3-f0ff-43ce-94ab-393f2e230bee.png)
  
__Months:__ When it comes to monthly trips, both casual and members exhibit comparable behavior, with more trips in the spring and summer and fewer in the winter. The gap between casuals and members is closest in the month of July in summer.   
__Days of Week:__ When the days of the week are compared, it is discovered that casual riders make more journeys on the weekends while members show a decline over the weekend in contrast to the other days of the week.  
__Hours of the Day:__ The members show 2 peaks throughout the day in terms of a number of trips. One is early in the morning at around 6 am to 8 am and the other is in the evening at around 4 pm to 8 pm while the number of trips for casual riders increases consistently over the day till evening and then decrease afterwards.  
  
We can infer from the previous observations that member may be using bikes for commuting to and from the work in the week days while casual riders are using bikes throughout the day, more frequently over the weekends for leisure purposes. Both are most active in summer and spring.  
  
Ride duration of the trips are compared to find the differences in the behavior of casual and member riders.  
  
![image](https://user-images.githubusercontent.com/125132307/230164787-3ea46ee9-aa5f-486b-9dd1-8f43dfce8e1c.png)  
![image](https://user-images.githubusercontent.com/125132307/230164889-1c7943d2-7ada-411b-adc7-a043eb480ba1.png)
  
Take note that casual riders tend to cycle longer than members do on average. The length of the average journey for members doesn't change throughout the year, week, or day. However, there are variations in how long casual riders cycle. In the spring and summer, on weekends, and from 10 am to 2 pm during the day, they travel greater distances. Between five and eight in the morning, they have brief trips.
  
These findings lead to the conclusion that casual commuters travel longer (approximately 2x more) but less frequently than members. They make longer journeys on weekends and during the day outside of commuting hours and in spring and summer season, so they might be doing so for recreation purposes.    
  
To further understand the differences in casual and member riders, locations of starting and ending stations can be analysed. Stations with the most trips are considered using filters to draw out the following conclusions.  
  
![image](https://user-images.githubusercontent.com/125132307/230248445-3fe69cbb-30a9-42c6-b5e8-ab433a620ff3.png)  
  
Casual riders have frequently started their trips from the stations in vicinity of museums, parks, beach, harbor points and aquarium while members have begun their journeys from stations close to universities, residential areas, restaurants, hospitals, grocery stores, theatre, schools, banks, factories, train stations, parks and plazas.  
  
![image](https://user-images.githubusercontent.com/125132307/230253219-4fb8a2ed-95e3-4e52-a359-9d86945b7a75.png)
  
Similar trend can be observed in ending station locations. Casual riders end their journay near parks, museums and other recreational sites whereas members end their trips close to universities, residential and commmercial areas. So this proves that casual riders use bikes for leisure activities while members extensively rely on them for daily commute.  
  
  
## Act
After identifying the differences between casual and member riders, marketing strategies to target casual riders can be developed to persuade them to become members.  
Recommendations:  
1. Marketing campaigns might be conducted in spring and summer at tourist/recreational locations popular among casual riders.
2. Casual riders are most active on weekends and during the summer and spring, thus they may be offered seasonal or weekend-only memberships.
3. Casual riders use their bikes for longer durations than members. Offering discounts for longer rides may incentivize casual riders and entice members to ride for longer periods of time.
