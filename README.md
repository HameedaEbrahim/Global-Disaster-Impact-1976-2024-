# Global Natural Disaster Impact (1976-2024)

## Overview: 
In this project, a comprehensive dataset of global disaster events is analyzed to explore how different hazards—such as earthquakes, floods, storms, wildfires, and other natural events—have affected populations across time and regions. The dataset provides detailed information including the type of disaster, start date, geography, severity indicators (such as total deaths or total affected), and in some cases additional measures like magnitude or intensity. This collection of variables allows for in-depth evaluation of both the occurrence of disasters and their human impact.
The aim of this analysis is to transform raw data into meaningful insights by examining long-term trends, seasonal patterns, severity classifications, and regional differences. Through techniques such as frequency analysis, and ratio calculations, the report highlights which areas are most at risk, which hazards are becoming more common, and how the impact on communities changes over years and quarters. These findings provide valuable knowledge that can support disaster preparedness, improve resilience, and contribute to more effective decision-making in risk management.

## Dataset Description:
Source: The International Disaster Database (EM-DAT)
Time period: 1976 - present
Rows: ~26K 
Columns: 46 

## Data Cleaning & Preparation: 
Cleaning steps included:
● Exlude some data: 
○ start the data from 1976 until 2024.

● Converted types of columns:
○ (Total Deaths, Total Affected, Start Month, Start Day) to integer. 
○ 

Python EDA Project

● Handled missing values:
○ (Start Day):
    1. Assume that the (start Day) = (End Day) 
    2. Drop the rows that the (Start Day) & (End Day)
○ (Start Month):
    1. Assume that the (start Month) = (End Month) 
○ (Total Affected, Total Deaths): 
    1. Drop the missing rows.
○ (Mgnitude): 
    1. Fill the magnitude for the earthquake disasters only.

● Created new Columns:
○ Date = Start Year , Start Month - Start Day 

● Fix the error in the Date: 
○ fix invalid date (e.g. Novmber have max date 30 , but in the data they put 31) 

● Drop columns: 
○ Drop the not important columns ( Entry Date, Last Update, ISO)

## Key Insights: 
1.


## Recommendations: 

## Tools & Libraries: 
● Python: pandas, numpy, calander.
● Tableau: for visuals.




