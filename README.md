# Fridays Tell the Story: How Remote Work Reshaped Commuting After COVID

## Introduction
The COVID-19 pandemic fundamentally changed how people live and work. With offices closed and remote work becoming common, daily routines and travel patterns shifted almost overnight.  
One of the most visible changes has been in commuting behaviour, particularly on Mondays and Fridays, as flexible work arrangements allowed more employees to work from home.  

This project investigates how commuting patterns have evolved in New South Wales (NSW) from 2020–2025, focusing on the **Friday ratio** — defined as **Friday patronage relative to the average Monday–Thursday patronage**.  
By analysing how this ratio has changed and identifying its drivers, we aim to uncover insights into post-pandemic travel habits and their long-term impact on public transport.

---

## Data Sources
We combined three datasets to analyse NSW public transport usage:

1. **Opal Patronage Data** — Hourly tap-on and tap-off counts from January 2020 to July 2025.
2. **Public Holidays** — NSW holiday dates obtained via the `holidays` Python library.
3. **Weather Data** — Daily weather conditions including rainfall, temperature, and wind.

---

## Methodology
1. **Data Cleaning & Integration**
   - Combined multiple Opal patronage files into a single dataset.
   - Added weather and public holiday features.
   - Created a Friday ratio metric for each week.

2. **Exploratory Data Analysis (EDA)**
   - Regional distribution of tap-on counts.
   - Long-term trends using rolling averages.
   - Seasonal trends and holiday effects.
   - Pre- vs Post-COVID comparisons.
   - Investigation into potential drivers of Friday decline.

3. **Modelling**
   - Tested regression models to identify factors influencing Friday ratio.
   - Included variables such as weather, seasonality, and holiday status.

---

## Key Findings
- **Post-COVID Shift** — Friday commuting remains consistently lower compared to midweek, indicating lasting remote work adoption.
- **Weather Influence** — Rain and extreme temperatures slightly reduce commuting levels.
- **Public Holidays & Events** — These significantly lower Friday patronage.
- **Long-Term Trend** — Friday ratio stabilised but did not return to pre-pandemic levels.

---

## Limitations
- Data only covers NSW, not national trends.
- Potential bias from events not captured in datasets.
- Weather data granularity may miss microclimate effects.

---

## Technologies Used
- **Languages:** R, Python
- **Libraries (R):** tidyverse, ggplot2, zoo, janitor, dplyr, ggpubr
- **Libraries (Python):** holidays
- **Tools:** RStudio, Jupyter Notebook

---

## Authors
- Huy Le Tran
- Cong Thanh Vu
- Minh Phuong Pham
