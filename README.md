# Module11Challenge
The task is to create:
1. A Jupyter notebook that clusters cryptocurrencies by their performance in different time periods.
2. Plot the results to visually show the performance to the board.

# Technologies
- python 3.8.15 (compatible with Prophet)
- JupyterLab
- libraries: pandas, hvplot, pathlib, prophet, numpy, holoviews, datetime
- MacOs
# Installation
If you want to run the program yourself and/or enter different data, do the following:
1. To install the project files, go to the GitHub page for the workshop, click on the green Code button, then download the repository as a ZIP file. 
<img width="1066" alt="image" src="https://user-images.githubusercontent.com/111472420/204167271-87f5b727-ea73-40cf-88ef-4c94a2acba17.png">

</br>
2. Unpack a zip file into the directory you can operate from in JupyterLab. 
<img width="1066" alt="image" src="https://user-images.githubusercontent.com/111472420/204167303-6ce208ec-2739-4676-8b0b-1a312f8aceb9.png">

3. Install all the libraries via Terminal, open forecasting_net_prophet.ipynb and Run the code!
<img width="1066" alt="image" src="https://user-images.githubusercontent.com/111472420/204167413-098ea1d6-215e-446a-b0df-ea462a5d05e1.png">

## Plotting the Results
### Step 1: Find Unusual Patterns in Hourly Google Search Traffic
![bokeh_plot (54)](https://user-images.githubusercontent.com/111472420/204167564-0b67502b-3ffd-41b8-b465-ce3b26b283dc.png)
</br>
<b>Question</b>: Did the Google search traffic increase during the month that MercadoLibre released its financial results? </br>

<b>Answer</b>: Yes, the Google search traffic increased during May 2020.
### Step 2: Mine the Search Traffic Data for Seasonality

![bokeh_plot (53)](https://user-images.githubusercontent.com/111472420/204167513-04d9399b-5860-4d04-86b5-4db93e1d7617.png) </br>

![bokeh_plot (55)](https://user-images.githubusercontent.com/111472420/204167635-be918a9e-de2e-41b6-a09e-419df283ac0a.png)
**Question:** Does any day-of-week effect that you observe concentrate in just a few hours of that day? </br>

**Answer:** That question's phrased very poorly. The weekends are less intense, so the hourly 'Search Trends' average is lower than on weekdays. 

</br>
<img width="726" alt="image" src="https://user-images.githubusercontent.com/111472420/204168880-df2229e2-bb12-48f6-8f60-9aea2a2ea75a.png">


 </br>

**Question:** Does the search traffic tend to increase during the winter holiday period (weeks 40 through 52)? </br>

**Answer:** The search traffic tends to increase during the winter holiday period as the trend line is ascending (week 41 through 51).</br>

### STEP 3: Relate the Search Traffic to Stock Price Patterns

![bokeh_plot (57)](https://user-images.githubusercontent.com/111472420/204167825-c00a26f0-e309-425e-b1a2-72e4200bceda.png) </br>

<img width="723" alt="image" src="https://user-images.githubusercontent.com/111472420/204167884-53b0abf3-3d65-479e-91b1-826290ce2e38.png"> </br>
![bokeh_plot (58)](https://user-images.githubusercontent.com/111472420/204167950-f0025d2c-66ee-4108-9cbd-b8e66fb34424.png) </br>
<img width="568" alt="image" src="https://user-images.githubusercontent.com/111472420/204167989-4748d239-c647-4463-a120-ac27d7621b12.png">
</br> </br>
**Question:** Does a predictable relationship exist between the lagged search traffic and the stock volatility or between the lagged search traffic and the stock price returns?
</br> </br>
**Answer:** No strong correlation exists between those variables. 

### Step 4: Create a Time Series Model with Prophet
<img width="736" alt="image" src="https://user-images.githubusercontent.com/111472420/204168073-b1353e26-aec2-4960-aa5f-5efe8316db26.png"> </br>
**Question:**  How's the near-term forecast for the popularity of MercadoLibre? </br> </br>

**Answer:** The popularity is going down. </br>
<img width="414" alt="image" src="https://user-images.githubusercontent.com/111472420/204168176-d7bae40d-8b8f-4719-97c8-4cf3c9f866cf.png">
</br>
![bokeh_plot (59)](https://user-images.githubusercontent.com/111472420/204168200-0db510bb-eeb2-41d8-9b78-ac5590833b21.png) </br>
<img width="706" alt="image" src="https://user-images.githubusercontent.com/111472420/204168242-d480bff3-358e-4b0e-a32f-d347696ab3f8.png">
<img width="706" alt="image" src="https://user-images.githubusercontent.com/111472420/204168282-c714657c-c382-4b3d-b9d6-552f73673657.png">
</br>
**Question:** What time of day exhibits the greatest popularity?
</br>
**Answer:** night-time </br></br>
**Question:** Which day of week gets the most search traffic? 
   </br>
**Answer:** Tuesday</br></br>
**Question:** What's the lowest point for search traffic in the calendar year?
</br>
**Answer:** # in October </br></br>
### Step 5 (Optional): Forecast Revenue by Using Time Series Models

![bokeh_plot (60)](https://user-images.githubusercontent.com/111472420/204168399-806c786f-efc0-429b-ab00-19664ad58f1d.png)
<img width="706" alt="image" src="https://user-images.githubusercontent.com/111472420/204168437-52daa4d0-2142-45ef-b6ca-62a75c0ce57f.png"> </br>
**Question:** For example, what are the peak revenue days? (Mondays? Fridays? Something else?) </br>

**Answer:** Wednesdays </br></br>
<img width="728" alt="image" src="https://user-images.githubusercontent.com/111472420/204168510-3e25621f-64c1-46fc-b40b-928c647b4dc9.png">
</br></br>
The trend for companie's total sales is ascending firmly. Most likely, the number for expected total sales next quarter will be $6920.11. Best case scenario - 8048.35, worst case - 5795.42.








