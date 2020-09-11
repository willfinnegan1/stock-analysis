# Stock-Analysis

## Overview 
The purpose of this analysis was to help a friend, Steve, gather stock market information specific to one publicly traded company, DAQO Energy and a number of other stocks in the energy space. As a follow up to the initial stock analysis i refactored the VBA code to run faster and more efficiently. 
 
 ## Results
 #### Stock Analysis
 Using images and examples of your code, compare the stock performance between 2017 and 2018, as well as the execution times of the original script and the refactored script.
 Analyzing the series of energy stocks for Steve has led me to several conclusions. In 2017, using the sample of 12 stocks, the energy sector performed well with 11 of 12 stocks (see figure 1) giving positive returns to shareholders. DQ notably was the top performing stock in the sample group in 2017, with a return of 199.4%.  While stock performance across the sample was great in 2017, 2018 did not provide positive returns for the majority of the sampled stocks (see figure 2). in 2018 DQ had a return of -62%, giving back a portion, though not all, of the gains made in 2017.
 
 #### Refactoring
the initial analysis was performed by creating an array of the 12 tickers (figure 3), and then using a loop to identify 3 variables for each ticker: 1) Volume 2) Starting Price 3) ending price (Loop code - see code in figure 4). I found this to be a simple way to pull the necessary data to provide % Return, and volume data to Steve to help inform his decision.

While the first pass got the job done, the coding was not the most efficient. To improve efficiency, i refactored the code. By setting ticker index variable = 0, and declaring Volume, Starting Price, & Ending Price each as a variable, the operator is able to use a for loop (figure 5) to comb through the data, and identify starting and ending prices. ending price determined when the following ticker does not match. By Refactoring we decreased the time required to run the macro (see figure 6). The new refactored code decreased run time by 76% and 82% for 2017 and 2018 respectively.

 
 ## Summary
 In summary, through refactoring the time required to run the macro was drastically reduced. In general, improving efficiency and speed is a good thing and a positve outcome. This is true as long as the process is still repeatable and interpretable. In this case, the benefit is negligible as each run took less than one second and Steven is only looking at two years of data.
 If this analysis were being done for a larger data set, on a larger set of historical data, perhaps for a securities trading firm, the benefit of refactoring would be great. When you apply efficiency gains to millions of transactions, the benefit is much more tangible. 
The refactoring excercise did improve efficiency, but will likely be unnoticed by the end user, Steve.



### Figure 1:
![](Resources/2017_Performance.png) 

### Figure 2:
![](Resources/2018_Performance.png)

### Figure 3:
![](Resources/ArrayCode_initialpass.png)

### Figure 4:
![](Resources/LoopCode_Initial.png)

### Figure 5:
![](Resources/Refactor_For_Loop.png)

### Figure 6:
![](Resources/RunTimeComparison.png)
