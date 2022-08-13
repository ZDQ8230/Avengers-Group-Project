# Quick Audit | Budget Calculator 


[![Presentation](Resources/Avengers%20Financial%20Presentation%20.gif)](https://www.canva.com/design/DAFI0GPv8Zc/yj4s6g1oZY8tkdylaFZh8A/view?utm_content=DAFI0GPv8Zc&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)



--

### `"What if I Invested my Savings?"`

--

# Overview: 

This project assess an individual's spending and saving using their bank statements. 

It is split into 4 sections Accordingly:

1. CSV Reader for Scrubbing and sorting Data for human readability
2. CSV Generator - Creates fake data for testing the program
3. Monte Carlo Simulation - Forecasts potential future Market Returns of US Stocks and Bonds
4. Research - Compare findings with Australian Benchmark 


## Outcome 


Using Financial technology including API, Monte-Carlos Stimulus, Python etc, the program can provide insights about:

- Personal Spending Habits
- Speculative Investment Return on personal saving 
- How do you compare with others within your age group



## Flow Chart


![Mind Map](./Resources/Flowchart.png)



# Technical Specifications

`Program uses multiple Python libraries. Dependancies include Faker, hvplot and matplotlib`

![Python Libraries](./Resources/libraries.PNG)


# Instructions:

## Part 1 - Analyze Cash Flow


### 1. Download bank statements as CSV

### Below are detailed instructions to download your CSV bank statements. It is recommnded that you download a year worth of recent data:

- [NAB](https://www.nab.com.au/personal/customer-support/using-online-banking-tools-to-make-tax-time-easier)
- [WESTPAC](https://www.westpac.com.au/business-banking/online-banking/support-faqs/export-detailed-transaction-history/)
- [ANZ](https://help.anz.co.nz/app/answers/detail/a_id/767/~/exporting-transaction-history)
- [COMMBANK](https://www.commbank.com.au/business/online-business-services/commbiz/faqs/how-to-export-transactions.html)

![Westpac Example](Resources/Westpac_Example.gif)





### 2. Set the file loaction for your csv file, and Run the CSV_reader


 Now you know your cash flow, you are better prepared to define your savings and investing goals 

## Results 

### Weekly Cash Flow Grouped By Year

The program makes it simple to see your expenditure and visualise your cashflow

![User Cash Flow](./Resources/cash_flow_chart.gif)


---


## Part 2 - Forecast Returns


### 2.1 Open the MC_Forecasting tool


### 2.2 Input you current age and retirement age 


### 2.2 Input Yearly Investment




## Results 

### Compare Savings to the Average Australian

![Savings Comparison Chart](./Resources/savings_comparison_chart.png)

#### Personal bankstatement
![](./Resources/Personal_saving_results_from_bankstatement%20.png)

- Shows top three savings
- Shows average yearly, monthly and weekly savings

### Show Investment Simulation

#### Encourage Saving and investing

![Results_MC_VS_Benchmark](./Resources/MC_Results.png)


---


## Data sorting, Cleaning and Exploration: 

Processing and cleaning data is essential as users are with different banks, thus have different bank statement formats (NAB, ANZ, CBA, Westpac). 

The CSV_Generator program models the "BIG 4" banks, as they are the prevelant financial institutions in Australia.

The Fake CSV's are used to demonstrate the application.

### Example of CBA bank statement: 
![CBA Bank Statement](./Resources/Example_CBA_statements.png)



### Example of ANZ bank statement: 
![ANZ Bank Statement](./Resources/Example_ANZ_statements.png)


### Example of Standardised DataFrame After Data Clean

![Dataframe](./Resources/bank_dataframe.png)



---

# Demo


![Demo CSV Gen](./Resources/CSV_Gen_demo.gif)
![Demo Reader](./Resources/CSV_GReader_demo.gif)
![Demo Simulation](./Resources/mc_forecast_demo.gif)

## Source of data: 

1. CSV Data extracted from user's bank statements. 

2. Analysis of historical data from S&P 500 and Aggregate Bond Index ETF,  obtained from Alpaca. 

    The data were then used for Monte-Carlos Simulations. 

    <sub>_Time period from 2017-05-01 to 2020-05-01_</sub>

3. Inflation data (Consumer Price Index, **CPI**) was obtained from Australian Bureau of Statistics (ABS). 

    Saving-By-Age data was obtained from Westpac. 

    <sub>_Time period for CPI was from Jun-2012 to Jun-2022._</sub>

    <sub>_Saving_By_Age was taken at 31-12-2020_</sub>



---
