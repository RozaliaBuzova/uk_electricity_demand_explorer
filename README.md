# UK Electricity Demand Analysis for 2025
![Python](https://img.shields.io/badge/Python-3.14-blue)
![Static Badge](https://img.shields.io/badge/Status-In_progress-orange)

## Project Overview & Data
<ins>**Aim:**</ins> Explore UK electricity demand in 2025. 

<ins>**Objectives:**</ins>
Identify:
- Daily and seasonal trends
- Peak demand
- Baseload demand 

<ins>**Data:**</ins> Half-hourly historic demand data from NESO (https://www.neso.energy/data-portal/historic-demand-data). 

## Technical Skills
<ins>**Python libraries:</ins>** matplotlib  |  pandas  

<ins>**Skills:</ins>** Hourly dataset handling  |  Datetime objects  |  Data visualisation

## Analysis
### Electricity Demand & Load Duration Curves

Figure 1 plots the half-hourly demand data to produce the electricity demand curve. 
Peak demand occurred on the 9 January and reached 48GW. 

It can be seen that in the winter months, demands close to the peak demand were reached on several occasions. 

In summer months, demand was markedly reduced. This reduction will further be explored by looking at moving averages. 

![Demand Curve](images/2025_electricity_demand_curve_with_peak.png)

Figure 1
<hr>

Figure 2 shows the load duration curve, with the absolute minimum demand identified as 17GW, defining the absolute baseload requirements for 2025. 

The figure also shows that in more than half of the year, demand exceeded 30GW. 

![Load Duration Curve](images/2025_load_duration_curve.png)

Figure 2
<hr>

### Average Daily Demand Variation

Averaged daily profiles are plotted in Figure 3. The absolute daily average profile (grey) is compared to the weekday and weekend profiles (teal and pink respectively). 

A marked reduction of ~5GW can be seen in the peak demand of weekdays in comparison to weekends. This is slightly more than 10% of the absolute peak demand of 48GW. 

![Weekday vs Weekend](images/2025_avg_daily_demands.png)

Figure 3
<hr>

Seasonal daily demand variation is shown in Figure 4. 

It can be seen that the demand peaks around 12pm and 5:30pm are roughly preserved in all seasons. 

Winter demand is shown to be significantly higher in comparison to other seasons and up to 10GW higher than in summer.

![Seasonal Daily Variation](images/2025_avg_daily_seasonal_demands.png)

Figure 4
<hr>

### Moving Average Trend Analysis

Finally, to identify seasonal trends, daily, weekly and monthly moving averages were calculated and plotted next to the raw demand curve profile. 

These smoothed curves identify the broader trends between days, weeks and seasons. 

The main trend observed, as expected, is a demand reduction in the summer months of about 10GW on average. This is also true for summer peak demands, which are shown to be more than 10GW lower than in winter, supporting previous findings from daily profile plotting. 

No significant daily or weekly trends are observed in the current plots and further analysis may be needed to identify these and support the differences identified in the average daily profile graphs. 


![](images/2025_moving_avg_analysis.png)

Figure 5
