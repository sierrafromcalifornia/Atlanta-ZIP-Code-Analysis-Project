![Zip Codes](./images/metro-atlanta-zip-codes-map.jpeg)


# Atlanta ZIP code Analysis Project

**Author**: Sierra Stanton

## Overview
![Github Repo Size](https://img.shields.io/github/repo-size/sierrafromcalifornia/dsc-phase-4-project?style=social)
![Github Follow](https://img.shields.io/github/followers/sierrafromcalifornia?style=social)
![Twitter Follow](https://img.shields.io/twitter/follow/sierrastanton?style=social)

This project analyses real estate data from Zillow Research to determine which areas are prime for investment. We have been charged with helping Hellbent Investments narrow down the ZIP codes that they should target as they plan for this next round of outspend. We'll use Zillow's dataset to dive into home values in Atlanta across time, and narrow down five ZIP codes worthy of investment according to project ROI.

## Business Problem

We' be forecasting real estate prices of various ZIP codes using data from [Zillow Research](https://www.zillow.com/research/data/). For this project, we'll will be acting as a consultant for Hellbent Investments, a real-estate investment firm focused on development in Atlanta, GA.

Hellbent Investments has asked me what seems like a simple question:

> What are the top 5 best ZIP codes for us to invest in?

In order to provide a solid recommendation, we met with the firm and determined that projected ROI across the next three years is the best way to narrow down the ZIP codes they'll want to focus on.

First, we'll investigate home value data across time within Atlanta's ZIP codes. Second, we'll investigate the ZIP codes themselves to gauge potential contributing factors. Third, we'll use time series forecasting via ARIMA and Facebook Prophet to chart out future home values and narrow down our list of ZIP codes to just five targets.

## Data

Data will be used from the following source:
* __[Zillow Research](https://www.zillow.com/research/)__ - this sector of Zillow aims to be the most open, authoritative source for timely and accurate housing data and unbiased insight.

Zillow Research's Zillow Data (`zillow_data.csv`): this dataset shows us the average housing sales prices in the United States based on location while shedding light on other location-focused aspects through rankings such as population density. This set shows us information on over 14,000 zip codes - let's explore it further.

## Methods & Results

I use descriptive analysis and time-series modeling to show:
* How the home values across Atlanta ZIP codes ranged over twenty-two years
* The population density across Atlanta ZIP codes
* The effect of the 08' housing crisis and how we narrowed data appropriately to downvalue this trend

Due to the datasets used and their current nature, I'm confident these findings will prove relevant as Hellbent Investments begins their next real-estate outspend. There are many more ways we can deepen our analysis to prove even more insightful with more time and access to additional data.

### Atlanta Home Values in 1998
![graph1](./images/viz_1.png)

### Atlanta Home Values in 2018
![graph2](./images/viz_2.png)

### Atlanta Home Values from 1998 - 2018
![graph3](./images/viz_3.png)

### Population Density Across Atlanta Zip Codes
![graph4](./images/viz_4.png)

### Atlanta Home Values from 1996 - 2018
![graph5](./images/viz_5.png)

### Atlanta Home Values from 2010 - 2018
![graph6](./images/viz_6.png)

## Conclusions

Here's how we estimate the strongest Atlanta ZIP codes will perform in the next two years:

1. `30308`: 24% return
2. `30316`: 16.5% return
3. `30331`: 15.7% return
4. `30317`: 9.3% return
5. `30363`: -2% return

## Next Steps

This goes beyond our initial time-series analysis and is worth further exploration.

Since we have fairly large confidence intervals for these ZIP codes and can't confidently say these will produce that return, I advise that we drill down even further into the top three ZIP codes and do the following:

**TECHNICAL**
1. Bring in our isolated data across ZIPS
2. Introduce further methods for stationarity
3. Tune our parameters according to our tests like ACF/PCF
4. Evaluate exactly which months were affected by the 08' crisis and remove them, while keeping data back to 96' which brings over a decade more of training data to improve our models
5. Bring in our holdout data for further evaluation betewen model iterations
6. Evaluate all of our Atlanta ZIPs versus the best past-performers to see how ROI and confidence levels compare

**NON-TECHNICAL**
Tie our research further to Hellbent’s Real Estate Development Goals by:
1. Diving deeper into Zillow’s metric for value determination through time, and ensure it matches the type of development and returns expected in context
2. Analyzing each ZIP code and creating a development project timeline and/or aligned metric to ensure we’re abreast of current development saturation - and how such past developments have affected housing values in Atlanta
3. Map ROI past a three year horizon in order to make increasingly actionable

We can use the same steps as shown here to evaluate different real-estate data given we have methods of assessing value and can therefore bring in comparable data to see how well our conclusions hold. We can even expand this to all or some of the other 14,000+ ZIP codes represented to develop more targets and evaluate predictability among returns.

## For More Information

Please review my full analysis in my [Jupyter notebooks](./notebooks) or [presentation](./presentation/Atlanta-ZIP-Code-Analysis-Project.pdf).

For any additional questions, please contact **Sierra Stanton** & stanton.sierraerin@gmail.com

## Repository Structure

```
├── README.md
├── notebooks
├── data
├── presentation
├── images
└── Atlanta_Zipcode_Analysis_Project.pdf
```
