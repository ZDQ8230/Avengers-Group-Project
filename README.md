# The Avengers Budget Calculator | Tool to encourage Saving & Investing

--

### "What if I put my savings into investment?"

--

# Overview: 

This project assess an individual's spending and saving using their bank statements. With FinTech (API, Monte-Carlos Stimulus, Python etc), we can provide insights about:

- Personal spending habits
- Investment return on personal saving 
- How does you investment return compare with inflation rate 
- How does you compare with others within your age group



## Mind Map 

![Mind Map](./Resources/Avenger_Budget_Calculator_Brainstorm.drawio%20(1).png)



# Technical 

## Source of data: 

In the input section, data was extracted from user's bank statements. 

In the analysis section, historical data of S&P 500 and Aggregate Bond Index ETF was obtained from Alpaca. The data were then used for Monte-Carlos Stimulus. 
- Time period from 2017-05-01 to 2020-05-01. 

In the output section, inflation data (Consumer Price Index, CPI) was obtained from Australian Bureau of Statistics (ABS). Saving-By-Age data was obtained from Westpac. 
- Time period for CPI was from Jun-2012 to Jun-2022. 
- Saving_By_Age was taken at 31-12-2020. 



------


## Data sorting, cleaning and exploration: 

Processing data is essential as users are with different banks, thus have different bank statements (NAB, ANZ, CBA, Westpac). 

 Example of CBA bank statement: 
![CBA Bank Statement](./Resources/Example%20of%20CBA%20bank%20statements.png)



Example of ANZ bank statement: 
![ANZ Bank Statement](./Resources/Example%20of%20ANZ%20bank%20statements.png)

Data was extracted from bank statements and used to build dataframe. 
![Dataframe](./Resources/bank%20dataframe.png)







