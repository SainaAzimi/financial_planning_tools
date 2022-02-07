![Financial Planner](Images/financial-planner.png)

# **Financial Planning Tools**
In this project you’ll create two financial analysis tools by using a single Jupyter notebook:

The first financial tool developed is a financial planner for emergencies. The members will be able to use this tool to visualize their current savings. The members can then determine if they have enough reserves for an emergency fund.

The second financial tool developed is a financial planner for retirement. This tool will forecast the performance of their retirement portfolio in 30 years and in 10 years. To do this, the tool will make an Alpaca API call via the Alpaca SDK to get historical price data for use in Monte Carlo simulations.

You’ll use the information from the Monte Carlo simulation to analyze if weighting the portfolio more heavily to stocks doesnt allow the members to retire after 10 years.


---
## Technologies
This application is developed on the *Python 3.7.11 version* 
Jupyter Lab Notebook that is an open sourced, web based user interface for software design, coding, visualization and documentationis is used for running the program that incorporates the following required dependencies:

**Pandas**: To import functions needed to program appliation for financial analysis

**%matplotlib**: To perform analyticals calculations

In this module, you’ll use the following Python modules and libraries to facilitate API requests:

**OS**: The OS module comes under Python's standard utility models and provides functions for interacting with the computer's operating system. The OS module does not require a separate download.

**Requests**: The Python Requests library helps you access data via APIs.

**JSON**: This library puts the response (that is, the data) from an API into a human-readable format.

**MCSimulation**:This is Python library named MCForecastTools which this file contains all the logic, in the form of Python code, that you need to run the Monte Carlo simulation. 

**dotenv**:With the python-dotenv library, you can read key-value pairs from an environment file (.env) and add them as environment variables.

**Alpaca**: Alpaca is an API for stock trading. With the Alpaca SDK, you can interact with the Alpaca API.


---
## Installation Guide

The following installation must be performed before running the program:

*Install Jupyter Lab*

*Install Pandas*

*Pip install python-dotenv*

*Pip install alpaca-trade-api*


---
## Usage
This section is an explanation of how to use this program: 

We start this application by importing all the necessary libraries, dependencies and data. Next, you will determine the current value of a member’s cryptocurrency wallet. You’ll collect the current prices for the Bitcoin and Ethereum cryptocurrencies by using the Python Requests library. 
Afterwards, you need to determine the current value of a member’s stock and bond holdings. You’ll make an API call to Alpaca via the Alpaca SDK to get the current closing prices of the SPDR S&P 500 ETF Trust (ticker: SPY) and of the iShares Core US Aggregate Bond ETF (ticker: AGG). Furthermore, you’ll use the valuations for the cryptocurrency wallet and for the stock and bond portions of the portfolio to determine if the credit union member has enough savings to build an emergency fund into their financial plan.
Finally, you’ll use the MCForecastTools library to create a Monte Carlo simulation for the member’s savings portfolio in two different situations: 
In the first situation, you run a Monte Carlo simulation of 500 samples and 30 years for the 60/40 portfolio, and then plot the results.
The next situation, you forecast the cumulative returns for 10 years from now. Because of the shortened investment horizon (30 years to 10 years), the portfolio needs to invest more heavily in the riskier asset—that is, stock—to help accumulate wealth for retirement.
Finally, you’ll use the information from the Monte Carlo simulation to analyze if weighting the portfolio more heavily to stocks doesnt allow the members to retire after 10 years.

---
## Contributors
*Contributors*: Saina Azimi

*Email*: azimi.sainaa@gmail.com

*LinkedIn*: https://www.linkedin.com/in/azimi-saina/ 

---
## License 
UC Berkeley
