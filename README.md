The DownMarketData project will look at the relationship between the S&P 500 and the 20+ Year US Treasury Bond. Throughout the history of the US Stock Market, when Stocks have a significant equity drawdown, Treasuries have been a much safer place to put your money. This year, for the first time, Treasuries, the risk-off asset, have had a larger decline than the stock market during a significant equity drawdown. This anamoly leads some professionals to believe that something troubling may be coming for the US economy.

Requirement 1: Loading Data - In Visual Studio Code, I read in APIs from https://www.alphavantage.co/documentation/ using a private API Key. I have hidden that API Key using a .env file and .gitignore so that it is not visible in my commits to GitHub. For the separate Tableau visualization, I found data online and created a spreadsheet that was used to create the side-by-side Bar Chart.

Requirement 2: Combine, Clean & Operate on the Data - I used pandas to clean up the datasets dropping columns, renaming columns, removing rows, converting a column of dictionaries into multiple columns, changing datatypes, etc. To combine datasets, I used an Outer Join merge so that they could be visualized on one chart.

Requirement 3: Visualize/Present the Data - In Visual Stuido Code, I used Line Charts to visualize the S&P 500 during the major stock market declines of 2008, 2020, and 2022 and did the same to visualize 20+ year Treasury Bonds during those same periods of time. Once the datasets were joined, I displayed the two on the same chart for each time period. In Tableau, I pulled the data from the spreadsheet to create a side by side Bar Chart showing how the S&P 500 and Treasuries compared during the 20 largest equity drawdowns between 1961 and the current year. It is easy to see that only the 2022 equity drawdown has an even larger decline in the 20+ year Treasury Bond. The link to the Tableau visualization is https://public.tableau.com/app/profile/troy.nally/viz/DownMarketData/Sheet2

Requirement 4: Best Practices - I created a Virtual Environment within Visual Studio Code to allow all of the necessary libraries and packages to be installed and imported.

Requirement 5: Interpretation of the Data - Each line of code is annotated with Markdown cells describing what the code is intended to do and why.

In order to run the program on your computer:

1. Open Visual Studio Code and use Python 3.10.6
2. Clone the Repository https://github.com/Monkeyorphan/DownMarketData.git
3. Open down_market.ipynb
4. Install pandas, requests, matplotlib, seaborn, and python-dotenv
5. Run All