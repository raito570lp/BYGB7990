# Portfolio Optimization
Given the uncertainty about the future performance of financial markets, investors typically 
diversify their portfolios to improve the quality of their returns. In this assignment, you
will be constructing a portfolio composed of two ETFs (exchange traded funds) that tracks
US equity and fixed income markets. The equity ETF tracks the widely followed S&P 500
while the fixed income ETF tracks long-term US Treasury bonds. We will use optimization
techniques to determine what fraction of your money should be allotted to each asset.

The Sharpe ratio is a widely used metric to gauge the quality of portfolio returns.
The higher the Sharpe ratio
value, the better the investment is considered to be. This formula assumes that returns are
normally distributed

###### Install R
We will use R to do the optimization.

In order to install R, we will go to https://cran.case.edu/
For IDE, we will use RStudio. https://rstudio.com/products/rstudio/download/

###### The steps
1. Upload the data in \asset data.txt" into R and call the tibble data.x.
Extract only the
observations where the federal funds rate is available (so you are left with
weekly data); this is the data you will use for the rest of the analysis. What
is the start date and end date of this reduced data set? Graph the federal funds interest
rate as a time series.

2. Now we will split the data into training and test sets.

3. The federal funds interest rate is in percent form so convert it to decimal (i.e., fractional)
form. Add both sets of returns to your training set
tibble. These returns are also called total returns. Construct a single time series plot
with the returns for both assets plotted.

4. Construct two normal quantile plot

5. Compute the correlation between the S&P500 and long term treasury bond returns in
the training set and interpret it

6. Compute the Sharpe Ratio

7. Write a function which takes the following inputs: (a) a vector of portfolio weights (call
this argument x; weights are between 0 and 1), (b) a vector of returns for asset 1, (c) a
vector of returns for asset 2, and (d) a vector of the corresponding weekly federal funds
interest rates.

8. Using the training set, use optimize() to determine the optimum weight for each asset using
the function you wrote in Question 7

9. Using all the steps we did before and evaluate our portfolio by testing the test set data.

10. How much would you have at the end of the test set period for each asset in addition to
the risk-free interest rate?
