# Tata-Business-Intelligence

## Project Overview
This project focus on exploratory data analysis of Tata business sales to generate business insights for the CEO and CMO on the following questions:

    - Which region is generating the highest revenue, and which region is generating the lowest?.
    - What is the monthly trend of revenue, which months have faced the biggest increase/decrease?
    - Which months generated the most revenue? Is there a seasonality in sales?
    - Who are the top customers and how much do they contribute to the total revenue? Is the business dependent on these customers or is the customer base diversified?


## Dataset
  Download the data [here](https://github.com/jims01/Tata-Business-Intelligence/blob/main/Online%20Retail%20Data%20Set.xlsx)

## Tool used
   Tableau [Download](https://www.tableau.com/en-gb)

## EDA process
  - The data was checked for duplicates to assure that I’ve provided the most up to date and error free analysis.
  - I removed all records with negative quantities or unit prices, as these entries would distort the analysis and needed to be excluded.
  - Calculated Revenue field and validity check.

Calculated Parameter
`` 
(IF [Show Top N or All] = 'All' THEN
    TRUE
ELSE
    RANK_UNIQUE(SUM([Revenue]), 'desc') <= 10
END) ``

## Result
1. The data indicates that revenue remained relatively stable during the first eight months, averaging around $685k. A significant increase began in September, with revenue rising 40% compared to the previous month. This upward trend continued through November, peaking at $1.5 million, the highest value of the year. December’s data is incomplete, so no conclusions can be drawn for that month.
2. The second visual highlights the top 10 countries with growth potential, excluding the UK due to its already high demand. Analysis shows the Netherlands, Ireland, Germany, and France generate high unit sales and revenue. These markets should be prioritized to further strengthen demand.
3. The third analysis examines the top 10 customers by purchase volume. Findings reveal minimal variation among them, with the highest-spending customer generating only 17% more revenue than the second. This indicates that revenue is not overly dependent on a few customers, suggesting low customer bargaining power and a strong market position for the business.
4. The map chart highlights regions with the highest and lowest revenue generation. Beyond the UK, countries such as the Netherlands, Ireland, Germany, France, and Australia show strong revenue performance, indicating investment potential to further increase demand. Most sales occur in Europe, with limited presence in the Americas and no demand in Africa, Asia, or Russia. Developing a targeted strategy for these underrepresented regions could significantly boost sales and profitability.

## Tableau Dashboard
[See Here](https://public.tableau.com/app/profile/adebayo.ajayi5142/viz/TATADASHBOARD/Dashboard1?publish=yes)














    
  
