# Quick Audit | Budget Calculator 


[![Presentation](Resources/Avengers%20Financial%20Presentation%20.gif)](https://www.canva.com/design/DAFI0GPv8Zc/yj4s6g1oZY8tkdylaFZh8A/view?utm_content=DAFI0GPv8Zc&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)



<br>


### `"What if I Invested my Savings?"`

<br>


<br>


<br>


# Overview: 

This project assess an individual's spending and saving using their bank statements. 

Using Financial technology including API, Monte-Carlos Stimulus, Python etc, the program can provide insights about:

- Personal Spending Habits
- Speculative Investment Return on personal saving 
- How does your finances compare with inflation rate 
- How do you compare with others within your age group



## Flow Chart

![Mind Map](./Resources/Mindmap.drawio.png)


<br>

<br>

<br>




# Technical Specifications

`Program uses multiple Python libraries including Faker, Pandas, Datetime, OS, Numpy and Pathlib `

![Python Libraries](./Resources/libraries.PNG)

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


## Data sorting, Cleaning and Exploration: 

Processing and cleaning data is essential as users are with different banks, thus have different bank statement formats (NAB, ANZ, CBA, Westpac). 

The program models the "BIG 4" banks, as they are the prevelant financial institutions in Australia.

### Example of CBA bank statement: 
![CBA Bank Statement](./Resources/Example_CBA_statements.png)



### Example of ANZ bank statement: 
![ANZ Bank Statement](./Resources/Example_ANZ_statements.png)


### Example of Standardised DataFrame After Data Clean

![Dataframe](./Resources/bank_dataframe.png)



---


## Create User Summary through Data Story

The program makes it simple to see your expenditure and visualise your cashflow

![Monthly Cash Flow Chart](./Resources/monthly_cashflow_chart.png)


## Show Investment Simulation to Encourage Saving and investing

`Insert chart of Monte carlo sim (Slice for period until retirement)`

## Compare Savings to the Average Australian

![Savings Comparison Chart](./Resources/savings_comparison_chart.png)



<br>


<br>

<br>




# Instructions:

## 1. Download bank statements as CSV

### Below are detailed instructions to download your CSV bank statements. It is recommnded that you download a year worth of recent data:

- [NAB](https://www.nab.com.au/personal/customer-support/using-online-banking-tools-to-make-tax-time-easier)
- [WESTPAC](https://www.westpac.com.au/business-banking/online-banking/support-faqs/export-detailed-transaction-history/)
- [ANZ](https://help.anz.co.nz/app/answers/detail/a_id/767/~/exporting-transaction-history)
- [COMMBANK](https://www.commbank.com.au/business/online-business-services/commbiz/faqs/how-to-export-transactions.html)

![Westpac Example](Resources/Westpac_Example.gif)

---

<br> 

## 2. Set the file loaction for your csv file and input the basic parameters

 ### 1. Set up file path to access your bank CSV 


<br>


### 2. Input you age, retirement age and risk appetite

<br>

### Code for input current age and expected retirement age
![Code for input current age and expected retirement age](./Resources/Age_and_retirement_age_input.png) 

<br>





### 3. Customise you investment return 



### Input risk appetite
![Code for input risk appetite](./Resources/risk_appetite_input.png)

<br>


## 4. View the results 

<br>

### Personal bankstatement
![](./Resources/Personal_saving_results_from_bankstatement%20.png)

<br>

### Monthly cash flow

![Monthly Cash Flow Chart](./Resources/monthly_cashflow_chart.png)

<br>

### User's saving in comparison to saving of his/her age group
![](./Resources/User_data_compare_to_saving_by_agegroup.png)
source: [Westpac](https://www.westpac.com.au/personal-banking/solutions/budgeting-and-savings/savings/savings-by-age/)

<br>


### Annualised return on investment in comparison to inflation rate 



