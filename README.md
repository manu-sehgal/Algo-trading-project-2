# Algo trading using Value investing strategy

For this project, we're going to build an investing strategy that selects the 50 stocks with the best value metrics out of SEP 500 stocks. From there, we will calculate recommended trades for an equal-weight portfolio of these 50 stocks.

We use IEX cloud's sandbox API to access the data through Batch API calling - a process which allows more interaction with less traffic and avoids throttle limit.

The goal of this strategy is to identify the 50 best value stocks from our data and then remove all the glamour stocks - all the remaining stocks outside the top 50.

using a function called portfolio_input, our program gets input for portfolio size, and generates recommendations accordingly

We can implement various different evaluation metrics like Price-to-earning ratio, price-to-book ratio, price-to-sales ratio, Enterprise Value divided by Earnings Before Interest (EV/EBITDA), EV/GA etc.

Some of these metrics aren't provided directly by the IEX Cloud API, and must be computed after pulling raw data
