# Global Natural Disaster Impact (1976-2024)

## Overview: 
In this project, a comprehensive dataset of global disaster events is analyzed to explore how different hazards—such as earthquakes, floods, storms, wildfires, and other natural events—have affected populations across time and regions. The dataset provides detailed information including the type of disaster, start date, geography, severity indicators (such as total deaths or total affected), and in some cases additional measures like magnitude or intensity. This collection of variables allows for in-depth evaluation of both the occurrence of disasters and their human impact.
The aim of this analysis is to transform raw data into meaningful insights by examining long-term trends, seasonal patterns, severity classifications, and regional differences. Through techniques such as frequency analysis, and ratio calculations, the report highlights which areas are most at risk, which hazards are becoming more common, and how the impact on communities changes over years and quarters. These findings provide valuable knowledge that can support disaster preparedness, improve resilience, and contribute to more effective decision-making in risk management.


## Dataset Description:
•	Source: The International Disaster Database (EM-DAT)
•	Time period: 1976 - present
•	Rows: ~26K 
•	Columns: 46


## Data Cleaning & Preparation: 
Cleaning steps included:
1.	Exclude some data: 
•	start the data from 1976 until 2024.
2.	Converted types of columns:
•	(Total Deaths, Total Affected, Start Month, Start Day) to integer. 
3.	Handled missing values:
•	(Start Day):
o	Assume that the (start Day) = (End Day) 
o	 Drop the rows that the (Start Day) & (End Day)
•	(Start Month):
o	Assume that the (start Month) = (End Month) 
•	(Total Affected, Total Deaths): 
o	Drop the missing rows.
•	(Magnitude): 
o	Fill the magnitude for the earthquake disasters only.
4.	Created new Columns:
•	○Date = Start Year , Start Month - Start Day 
5.	Fix the error in the Date: 
•	fix invalid date (e.g. November have max date 30 , but in the data they put 31) 
6.	Drop columns: 
•	Drop the not important columns ( Entry Date, Last Update, ISO)


## Key Insights: 
1.	Natural hazards now dominate global disaster frequency.
2.	Floods, storms, and earthquakes hazards account for the majority of natural disasters.
3.	Floods occur most frequently in Summer, driven by monsoon rainfall and high evaporation.
4.	China has the highest flood risk index
5.	Storms peak in Autumn, aligning with typhoon and hurricane season.
6.	Philippines ranks highest in storm risk.
7.	Earthquakes show no seasonal pattern, as expected for tectonic activity.
8.	China ranks highest due to major fault systems and active plate boundaries.
9.	Higher magnitude in earthquakes = exponentially more energy released.
10.	Most earthquakes occur around the Pacific Plate (Ring of Fire).
11.	Disasters without response have significantly higher death tolls.
12.	Asia is the most underserved region despite having the most disasters.


## Recommendations: 
# For flood disasters: 
    1.	Strengthen early-warning and evacuation systems.
    2.	Improve drainage, riverbank reinforcement, and urban water flow.
    3.	Prioritize high-risk countries for seasonal preparedness.
# For storm disasters: 
    1.	Develop region-specific seasonal forecasting and communication.
    2.	Enhance coastal protection and shelter infrastructure.
    3.	Develop preparedness efforts.
    4.	Expand community-level training and early-alert coverage.
# For earthquake disasters: 
    1.	Implement and enforce seismic-resistant building standards.
    2.	Prioritize regions with high deaths per event.
    3.	Expand public awareness programs and emergency drills.
# For response: 
    1.	Improve response coordination: Countries and organizations should enhance disaster response planning to ensure rapid mobilization after appeals.
    2.	Prioritize high-risk areas: Use historical disaster data to identify regions with frequent disasters and high affected numbers, and allocate resources proactively.
    3.	Strengthen early warning systems: Especially for floods and storms, improved forecasting and communication can reduce casualties.
    4.	Capacity building: Train local authorities and volunteers in emergency response to improve response effectiveness.


## Tools & Libraries: 
● Python: pandas, numpy, calander.
● Tableau: for visuals.




