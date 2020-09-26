# Stock-Analysis Project

## Overview of Project

### Purpose and Background

This project was initiated to determine if refactoring the VBA code from a previous stock analysis program would improve the functionality, specifically run time
, of the stock analysis routine. The initial project was a stock analysis program that analyzed data for 12 stocks in either the year 2017 or 2018. The first script
made use of the mutable nature of variables to determine the traded volume of each stock over the year and the annual return of each stock. The refactored code
was designed to make use of the array data type. This report is a discussion of how using arrays optimized the run time of the code.

## Results and Summary

### Results

The refactoring of the stock analysis code was designed to make use of the array data types and different indexed locations to store data for each stock via the
stocks tickers. The first step of the process was to initialize a variable to use as a record of a current ticker index location.

![Initalizing the arrays and index counter for the stock analysis](https://github.com/MattK1454/stock-analysis/blob/master/Resources/Code%20Part%201.png)

The next step in the stock anaysis was to replace the use of variable mutation to track the data of the stock with the indexed value associated with each stock.
This used the same looping logic as the intial code but altered the storing of the values of the stock volumes, startingPrice, and endingPrice in indexed locations
of each specified array.

![Looping logic using array index locations](https://github.com/MattK1454/stock-analysis/blob/master/Resources/Code%20Part%202.png)

The final section of code is used to format the output of the data using indexed location for each array.

![Code for formatting the output of the data pulling from values stored in arrays](https://github.com/MattK1454/stock-analysis/blob/master/Resources/Code%20Part%203.png)

### Summary
