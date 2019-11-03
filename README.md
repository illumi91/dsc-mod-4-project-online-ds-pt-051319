# Time Series Project on Zillow Database by Luigi Fiori

## Files 

- zillow_data.csv: Raw Data
- mod_4_starter_notebook.ipynb: Notebook for Analysis
- presentation_zillow.pdf: Slide presention

## Introduction

We need to perform a Time Series analysis on a Zillow database, an american online real estate database company.

![https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/246x0w.jpg](https://github.com/illumi91/dsc-mod-4-project-online-ds-pt-051319/blob/master/zillow%20project/246x0w.jpg)

Our goal is to formulate a Time Series analysis such that we can get some valuable insights for a potential company.
In particular we have been asked to find the 5 best Zip Codes, in Kansas City, in terms of potential investment for a 3 years period of time.

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

