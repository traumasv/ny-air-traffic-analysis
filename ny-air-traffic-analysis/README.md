# Data Management and Analysis Project

## 1. Documentation

### Project Description

Analysis of flight departure performance for the airports in the Greater New York Area in December of 2018

### Data Source or Description of Data 
Data Set: Reporting Carrier On-Time Performance (Decemeber 2018)

Data Source: Bureau of Transportation Statistics

URL: https://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=236

### Field and / or Columns and Their Types

* FL_DATE : `datetime` - Flight Date (yyyy-mm-dd)
* OP_UNIQUE_CARRIER : `object` - Unique Carrier Code
* OP_CARRIER_FL_NUM : `int` - Unique Flight Number
* ORIGIN : `object` - Acronym of the Airport of Departure
* DEST : `object` - Acronym of the Airport of Arrival
* CRS_DEP_TIME : `object` - Expected Departure Time
* DEP_TIME : `object` - Actual Departure Time
* DEP_DELAY_NEW : `float` - The time of delay for departure (0 if early or on time)
* CRS_ARR_TIME : `object` - Expected Arrival Time
* ARR_TIME : `object` - Actual Arrival Time
* ARR_DELAY_NEW : `float` - The time of delay for arrival (0 if early or on time)
* CANCELLED : `float` - Status of Flight (if cancelled)
* CANCELLATION_CODE : `object` - Reason for Cancellation
* CARRIER_DELAY : `float` - Carrier delay in mins
* WEATHER_DELAY : `float` - Weather delay in mins
* NAS_DELAY : `float` - National Air System delay in mins
* SECURITY_DELAY : `float` - Security delay in mins
* LATE_AIRCRAFT_DELAY : `float` - Late Aircraft delay in mins

## 2. Diagram / Sample Documents and Collections

![ER Diagram](er-diagram.png)

## 3. Data Import and Collection... or Data Generation

[Data Import](https://github.com/nyu-csci-ua-0480-003-fall-2019/traumasv-mini-project/blob/1cd405f17564cafb67d6cac3c79c8aede68837ff/cleaning_and_analysis.ipynb#L242)

## 4. Analysis

* create a column called total departure delay time using list comprehension
* use higher order function to find the date with the greatest avg departing delay time
* create a column to find the total delay (departure + arrival) using list comprehension

[Creating Total_Departure_Delay Column](https://github.com/nyu-csci-ua-0480-003-fall-2019/traumasv-mini-project/blob/1cd405f17564cafb67d6cac3c79c8aede68837ff/cleaning_and_analysis.ipynb#L288)

[Creating Total Delay (Departure + Arrival)](https://github.com/nyu-csci-ua-0480-003-fall-2019/traumasv-mini-project/blob/1cd405f17564cafb67d6cac3c79c8aede68837ff/cleaning_and_analysis.ipynb#L306)

## 5. Research

* [Documentation to Seaborn](https://seaborn.pydata.org/tutorial/distributions.html#plotting-univariate-distributions)
* Using Seaborn to simply visualize the pattern of the average departure delay time throughout the month
* [Using Seaborn to Plot the Avg Delay](https://github.com/nyu-csci-ua-0480-003-fall-2019/traumasv-mini-project/blob/1cd405f17564cafb67d6cac3c79c8aede68837ff/cleaning_and_analysis.ipynb#L566)

