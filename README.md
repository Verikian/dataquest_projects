# Dataquest Projets

Guided projects made as part of the *Data Analyst in Python* path.


## EN Description

### Analysis of eBay Car Sales Data
The project is in the file `Exploring_Cal_Sales_on_German_eBay.ipynb` and is using `autos.csv` dataset. 
This dataset can be found [here](https://data.world/data-society/used-cars-data). 
The goal of this project was to clean and analyze the data of used cars from [eBay Kleinanzeigen](https://www.kleinanzeigen.de/), a classified section of the German eBay website.

The project consists of:
- cleaning the data (clean column names, translate German words, convert values stored as text to numeric values, remove entries with outliers and incorrect data),
- exploring price by brand,
- analyzing mileage for the top 9 brands,
- discovering the most common brand-model combinations.

Analysis summary:
- The site consistently crawled data each day from `2016-03-05` to `2016-04-07`.
- After removing outliers, the mean price of cars is equal to `$5722`.
- There are some incorrect values in `registration_year` column (cars registered many years before cars were invented, or registered many years into the future).
- On average, among the top 9 brands (with at least 2% share in the dataset), the most expensive are: **Audi** ($9094), **Mercedes Benz** ($8484), **BMW** ($8103).
- On average, among the top 9 brands, the least expensive are: **Renault** ($2395), **Opel** ($2877), **Peugeot** ($3039).
- The average mileage values for each brans are in the range $116000 - $133000. There isn't any clear pattern in the mean price values, given the mileage values.
- The most common brand-model combinations are: **Volkswagen Golf**, **BMW series 3**, **Opel Corsa**.

<br>
### Heavy Traffic Indicators on I-94
The project is in the file `Heavy_Traffic_Indicators_on_I-94.ipynb` and is using `Metro_Interstate_Traffic_Volume.csv` dataset.
This dataset can be found [here](https://archive.ics.uci.edu/dataset/492/metro+interstate+traffic+volume).
The goal of this project was to analyze westbound traffic on the east-west [I-94 Interstate Highway](https://en.wikipedia.org/wiki/Interstate_94) connecting the Great Lakes and the northern Great Plains regions of the United States.

The project consists of:
- dividing the dataset into two parts (daytime and nighttime),
- analyzing time influence for each part (month, day of the week, time of day),
- analyzing weather indicators for each part.

For daytime data the following traffic indicators has been found:

**Time indicators**:
- The traffic is heavier during warm months (March - October) compared to cold months (November – February).
- The traffic is heavier on business days compared to the weekends.
- On business days, the rush hours are around 7 and 16.

**Weather indicators**:
- Shower snow.
- Light rain and snow.
- Proximity thunderstorm with dizzle.

For nighttime data the following traffic indicators has been found:

**Time indicators**:
- The traffic is heavier during warm months (March – October) compared to cold months (November – February).
- After 3 o'clock the traffic is heavier on business days. Between 21 and 3 it's heavier during the weekends.
- On business days, the rush hours are in the morning (between 5 and 6).
- On business days, after 19 o'clock, the highest traffic is on Friday.
- During the weekends, after 19 o'clock, the highest traffic is on Saturday.

**Weather indicators**:
- Proximity shower rain.
- Light intensity shower rain.

<br>
### Euro Daily Exchange Rates
The project is in the file `Storytelling_Exchange_Rates.ipynb` and is using `euro-daily-hist_1999_2020.csv` dataset.
This dataset can be found on [Kaggle](https://www.kaggle.com/datasets/lsind18/euro-exchange-daily-rates-19992020). 
The data source is the [European Central Bank](https://data.ecb.europa.eu/data/datasets/EXR/data-information). This dataset gets regular updates. 
The goal of this project was to analyze and visualize daily exchange rates between Euro-USD, Euro-Franc, and Euro-Yuan during coronavirus pandemic.

The project consists of:
- cleaning the data (renaming columns, changing the `time` column to a `datetime` data type, sorting values),
- showing long-term trends for exchange rates using the rolling mean (aka the moving average),
- showing Euro-USD, Euro-Franc, and Euro-Yuan exchange rates during the coronavirus pandemic with `2016-2019` period as a baseline,
- showing exchange rates in `2020` relative to `2020-01-02 ` between the euro and other currencies.

Analysis summary:
- The dataset consists of 5699 rows. Each row is a single day between `1999-01-04` and `2021-01-08`.
- The rolling mean for 30-day time interval has been chosen to show long-term trends for exchange rates.
- Euro-USD rate increased rapidly during coronavirus pandemic in 2020.
- Euro-Franc rate slightly decreased at the beginning of coronavirus pandemic in 2020.
- Euro-Yuan rate increased during second wave of coronavirus pandemic in 2020.

<br>
Code has been written in **Python** using **Jupyter Notebook**.

Libraries used in projects:
- `numpy` and `pandas`: for data analysis
- `matplotlib`: for visualizing data

Tested on `Python 3.10.12`.
