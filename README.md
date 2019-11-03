# Time Series Project on Zillow Database by Luigi Fiori

## Files 

- zillow_data.csv: Raw Data
- time_analysis_notebook.ipynb: Notebook for Analysis
- presentation_zillow.pdf: Slide presention

## Introduction

We need to perform a Time Series analysis on a Zillow database, an american online real estate database company.

![https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/246x0w.jpg](https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/246x0w.jpg)

Our goal is to formulate a Time Series analysis such that we can get some valuable insights for a potential company.
In particular we have been asked to find the 5 best Zip Codes, in Kansas City, in terms of potential investment for a 3 years period of time.

![https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/Kansas_City_Principal_Streets_and_Zip_Codes.png](https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/Kansas_City_Principal_Streets_and_Zip_Codes.png)

We'll be following the OSEMN methodology:

1.Obtain-->Filtering our data for chosen Zipcodes in Kansas City

2.Scrub--->we'll reshape our dataframe and in addition, we'll set the time column as our index to allow easy manipulation of our data

3.Explore->Plotting our data allows us to identify the peaks and fails, trends and even noise.

4.Model---> -Detrend the time series using differencing
            -Try several p, d, q parameters
            -Fit the model
            -Calculate MSE
            -Decide the AR,I, MA, and order of these models based on the lowest MSE

5.Interpret->Obtain valuable Insights and give raccomandations


# 1. OBTAIN

We are going to load our Data in a Pandas DataFrame in ordet to use and manipulate our data in a more efficient way.

![https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/df.PNG](https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/df.PNG)


Next step we'll be filtering our data so that we gonna have just the Zip Codes for Kansas City.

![https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/filter.PNG](https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/filter.PNG)


# 2. 3. 4. SCRUB, EXPLORE AND MODEL

Through our for loop we manage to melt our data in a Pandas DateTime so that we can use it and create a Time Series.

Subsequently we try several parameters in order to obtain an ARIMA model with the lowest MSE.

![https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/ARIMA.PNG](https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/ARIMA.PNG)


# 5. INTERPRET RESULTS

![https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/1000000.PNG](https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/1000000.PNG)

Here we caan see the 5 Best Zipcodes for our analysis.

We have selected the 5 Zip Codes with the highest ROI.

Moreover I added a column with a potential value over 3 years for a Million dollas investment.

![https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/zips_graph.PNG](https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/zips_graph.PNG)

Let's now plot a map with the precise location of the Zip Codes.

![https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/Capture.PNG](https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/Capture.PNG)

As we can see all these zipcodes result pretty remunerative in a 3 years period and from the graph above we notice a linear upward trend for all of them.

The ROI is almost identical for these 5 Zip Codes so we advice to differentiate the investment not only as said before on the location of the Zip Code, it's interesting to notice in fact that we are in the condition of investing on different potential targets of people, young couples or single people for example, based on the property prices. 

Prices are ranging from 100000 for the Zip Codes 66106, 66103 to over 300000 for the Zip Code 64112 making our strategy potentially wide and effective. 
