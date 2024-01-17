#Module 4 Challenge-Portfolio Analysis#

Objective:  The objective of the challenge is to create the code utilizing different python and pandas’ tools to analyze investment portfolios and perform a risk return analysis against the SP500 index benchmark to evaluate their performance.

The file with the code used to analyze the different portfolios and their  results is located in the DATA folder  under “Whale_analysis.ipynb”  

##Prepare the Data##

Before any analysis is done the code will import the relevant panda libraries that will be used for the calculations.  The code is set up to read the first read the CSV files containing the daily returns of the Whale and Algo Portfolios and the SP500 closing prices to create the data frame that will be used for the risk and return analysis.  Before the data frame is created, the code is set up to read the files and clean the data, making sure it is in the right type and dropping any null and removing any non-numeric values in the entries.  For the SP500 closing process, the daily returns will be calculated using the percentage change formula.  The code will also set up the files with the correct time index to create the concatenated data for the daily returns that will be used to perform the statistical and financial variables to determine their performance using the SP500 as the benchmark.

###Perform Quantitative Analysis###
Performance and risk analysis are calculated for each portfolio using the daily returns, cumulative and calculating, standard deviation, covariance, correlation, Beta, rolling 60-day beta and annualized Sharpe ratios.  To help in the evaluation of the performance and risk, the results are presented in different graphs such as plots, box plots and bars for each portfolio and then evaluating them against the SP500 benchmark. Also, an exponentially weighted average of 21 days for the standard deviation of the portfolios is calculated and plotted as further insight into the evaluation of the risk and performance of each portfolio. (1)(2)

###Create a Custom Portfolio###

For this sections new CSV files are made with the investment instruments data in the custom portfolio   to be readable.  The custom portfolio the is then cleaned and, after the daily return is calculated using a weighted return assuming an equal number of shares for the custom portfolio, the results are added as a new column to existing concatenated data frame containing the Whale, Algo an SP500 daily returns.

The code will then calculate and in some cases graph a similar a similar risk return analysis showing the annualized standard deviation, a rolling 21-day standard deviation, correlation, 60-day Beta and Sharpe ratios of the stocks to be compared with the SP500. The custom portfolio analysis will also provide graphs to facilitate the comparison against the SP500 benchmark.  Please note the results of the custom portfolio analysis will be based on the data timeframe of the custom portfolio which is different from the analysis performed in the initial Whale and Algo portfolios.  As a result, the overall performance of the each of the portfolios will be different once compared with Custom Portfolio and the SP 500 benchmark.


###Resources###
(1)	https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.ewm.html
(2)	Tutoring session Fintech Bootcamp-Berkeley 
(3)	UCB-VIRT-FIN-PT-12-2023-U-LOLC Python and Pandas in class exercises.
