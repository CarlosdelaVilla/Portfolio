🚖 Chicago Taxi Trip Analysis
Project Overview

This project analyzes taxi trip data from the city of Chicago to identify travel patterns, compare taxi company performance, and evaluate how weather conditions impact travel times to one of the city's busiest destinations: O'Hare International Airport.

Using SQL-generated datasets and Python for data analysis, this project combines exploratory data analysis (EDA), data visualization, and statistical hypothesis testing to generate actionable business insights.

Business Problem

A ride-sharing company wants to better understand customer demand and operational performance within Chicago. By analyzing historical trip data, the company aims to identify high-demand neighborhoods, evaluate the market share of taxi companies, and determine whether adverse weather conditions significantly affect travel times to the airport.

The insights can support strategic decisions related to fleet allocation, pricing, and customer expectations.

Project Objectives
Analyze taxi company performance based on total trips completed.
Identify the most popular drop-off neighborhoods in Chicago.
Visualize travel demand using informative charts.
Investigate whether rainy weather impacts travel time between Downtown Chicago (The Loop) and O'Hare International Airport.
Validate findings using statistical hypothesis testing.
Dataset

The project uses three SQL-generated datasets:

1. Taxi Companies

File: sql_result_01.csv

Contains:

Taxi company name
Number of trips completed on November 15–16, 2017
2. Drop-off Locations

File: sql_result_04.csv

Contains:

Chicago neighborhood
Average number of trips ending in each neighborhood during November 2017
3. Airport Trips

File: sql_result_07.csv

Contains:

Pickup timestamp
Weather conditions
Trip duration (seconds)

This dataset is used to evaluate the effect of weather on airport travel times.

Project Workflow
Data Preparation
Imported CSV datasets
Verified data types
Performed data validation
Explored dataset structure
Exploratory Data Analysis (EDA)
Compared taxi companies by trip volume
Identified the Top 10 Chicago neighborhoods by average drop-offs
Created visualizations to identify market trends
Generated business insights from each analysis
Statistical Analysis

Performed an independent two-sample t-test to evaluate whether rainy Saturdays significantly affect travel time from The Loop to O'Hare International Airport.

Hypothesis Testing

Null Hypothesis (H₀):

The average trip duration from The Loop to O'Hare is the same on rainy Saturdays and non-rainy Saturdays.

Alternative Hypothesis (H₁):

The average trip duration from The Loop to O'Hare is different on rainy Saturdays.

The hypothesis was tested using an independent two-sample t-test with a predefined significance level (α).

Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
SciPy
Jupyter Notebook
SQL
Key Business Questions
Which taxi companies completed the most trips?
Which Chicago neighborhoods receive the highest number of drop-offs?
How is market demand distributed across the city?
Does weather significantly impact airport travel times?
What operational insights can support better fleet management?
Repository Structure
Chicago-Taxi-Trip-Analysis/
│
├── README.md
├── requirements.txt
├── LICENSE
├── data/
├── images/
├── notebooks/
└── sql/
Future Improvements
Build a predictive model for trip duration.
Incorporate real-time weather information.
Analyze demand patterns by hour and weekday.
Develop an interactive dashboard using Power BI or Tableau.
Explore geospatial visualizations of pickup and drop-off locations.