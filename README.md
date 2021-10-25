 # Analysis of COVID-19 Infection Trajectory of Dane County, WI using Rolling Average.
  ## For code and graphs navigate to main.ipynb
  ## This analysis uses public data from the Wisconsin Department of Health Services. We will be specifically looking at positive cases that are reported daily and using a rolling average to determine the trend of new positive cases in the near future. 
  ### Rolling Average Definition: (statistics) a derived sequence of the averages of successive subsequences of a given number of members, often used in time series to even out short-term fluctuations and make a trend clearer. 
  ### Example: Suppose we wanted to apply a 3-day rolling average on a sequence of numbers (1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21,...)
  ### By definition a "3-day rolling average" is a derived sequence of the averages (i.e divide by 3) of successive subsequences of 3 members (i.e (1, 2, 3), (2, 3, 4), (3, 4, 5), (4, 5, 6), (5, 6, 7),...)
  ### Thus, we have 
  ###    (1+2+3)/3=2, 
  ###    (2+3+4)/3=3,
  ###    (3+4+5)/3=4,
  ###    (4+5+6)/3=5,
  ###    (5+6+7)/3=6,
  ###    (6+7+8)/3=7,
  ###    (7+8+9)/3=8,
  ###     .... so on and so forth
  ### Our derived sequence is thus (2, 3, 4, 5, 6, 7, 8, 9, 10,...)
  
  ## Graph 1: 
  ### Positive new cases plotted as vertical bars with a 7-day rolling average plotted as a line for 2020.
  ## Graph 2: 
  ### Positive new cases plotted as vertical bars with a 7-day rolling average plotted as a line for 2021.
  ## Graph 3: 
  ### Prediction of next 30 days, given positive new cases with a 30-day rolling average plotted as a line for 2020-2021.
  ## Notes: 
  ### 1. prediction() can take any number of days you want to predict and any number of days for the rolling average. It will give you insight as to whether there will be an increase or decrease in positive new cases based on previous data that is available.)  
  ### 2. The graphs produced use time series based on the number of days where data is available, if you use this code to generate a graph, dont forget to change inputs for the number of days where there is data available. Any dataset can be used in the predictor function; variables can be changed based on your own dataset. 
  
  
