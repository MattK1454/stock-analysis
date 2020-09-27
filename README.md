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

When discussing the refactoring code it is important to detail the pros and cons of the practice. One of the primary benefits of refactoring code is that the code
can be made to run more efficiently consuming less processing power, and memory resources. Should refactoring be performed properly, the code can run faster and
can be used to perform tasks in less time achieving the correct results. By refactoring code, or restructuring how the logical tasks of the code are performed, 
there is a possibility the newly restructed code can achieve the ideal results using less resources. However, there is a negative aspect to the refactoring of 
code. If the code is restructured improperly, carrying out of the desired logical tasks can actually use more resources and even return erroneous results. This 
would mean that leaving the code as it was before would have been the optimal solution as restructuring the code incorrectly would result in using more computing 
resources to achieve incorrect results.

When discussing the refactoring of the stock analysis VBA code, the distinct advantage of refactoring this specific code is the improved run time.

2017 refactored run results
![2017 refactored run results](https://github.com/MattK1454/stock-analysis/blob/master/Resources/VBA_Challenge_2017.png)

2018 refactored run results
![2018 refactored run results](https://github.com/MattK1454/stock-analysis/blob/master/Resources/VBA_Challenge_2018.png)

In the previous code, the average run time lasted at least 0.25 seconds longer. My understanding of why the original code ran took longer is because 
of the need in the original code to reset the values of variables used to track the values of volume, starting, and ending prices for each ticker index value. 
The advantage of the refactored code is that the memory used is all allocated to a singular array data type allowing the values to be adjusted in a way that 
reduced the need to reset values to performed the desired logic tasks. Rather, the logic made use of the values stored in a singular array memory location. The 
refactored code makes use of an indexed location via a variable value that is adjusted to allow for specific indexing within arrays. A disadvantage of this 
refactored code is that it becomes more complex in nature. If the code is not commented and understood then it becomes more complex for another person to 
adjust, and utilize the stock analysis code. The code, refactored properly, runs more efficiently. The disadvantage of the stock analysis code is that the logic 
must be well understood if it is to be adjusted or utilized to analyze adjustments in the source data. 

## References

1. Module 2 Challenge. (n.d.). Retrieved September 26, 2020, 
from https://courses.bootcampspot.com/courses/453/assignments/5582?module_item_id=78762

2. Find Your&nbsp;. (n.d.). Retrieved September 27, 2020, 
from https://www.citationmachine.net/apa/cite-a-website
