It is a Work in Progress!
Work done so far: 

Dataset given: Electricity consumption in Morocco measured at 10 minute intervals across 3 zones, including environmental factors such as temperature, humidity, and wind speed.

Objective: You've been hired as a demand analyst for Morocco National power grid co. 
The power grid is assessing plans for upgrading its infrastructure. You've been asked to assess seasonality in electricity consumption, to identify peak load periods across hours of the day and days of the week to help make investments to avoid outages during these hours. 

Project Goal: 
Assess electricity demand patterns across time and zones to identify:
Peak load periods 
High-risk congestion windows
Seasonal and intraday demand behavior
Intra year risk analysis to support infrastructure investment and outage prevention planning.

Analysis Pipeline: 
Data exploration → Data cleaning and engineering → Measures and Metric → Visualising

Core Analysis: 
National load trends
Hourly and weekly seasonality
Peak load windows
Zone contribution to peaks
Load volatility

Supporting analysis: 
Temperature, wind speed, DiffuseFlows and humidity correlation to consumption. 
Policy-level insight

Data Engineering: 
I normalized the single table CSV file into a star schema to support scalable time based and zone based analysis. Unpivoted the Zone column for ease of use and adding on measures later on. 

Measures Created: 
National Consumption
Average National COnsumption
Average Load
Peak Load
Load Above Average
Peak Load Flag: For peak load flags, As per industry standard, a heuretic of 1.25 is used in the formula to identify significant spikes. Meaning, If the current power consumption is 25% higher than the average, it is flagged as a Peak Load (1), otherwise it's normal (0).
Average Load by Hour
Average Load by Day of Week
Seasonality Analysis: Are there recurring high-load periods across the year that justify long-term infrastructure investment? 
