# 🥤Affordability of Coke Around the World🥤
This is a project that calculates the affordability of Coke.

*Read the story here: [Is Coke Affordable in Your Country?](https://xinyitu.github.io/coke-index/)*
## Goal
If you've lived in different countries in your life, one thing that you would inevitably notice is prices. Living in the United States while living on earnings in the developing world is difficult, as things such as food and services are usually more expensive here than my home country. 

As a sweet tooth who can't resist the charm of fizzy, bubbly carbonated drinks, I want to calculate the affordability of Coke around the world and see if it can refelct a country's cost of living or income level.

## Data Collection
- I scraped world [Coke local prices](https://www.numbeo.com/cost-of-living/country_price_rankings?itemId=6) and [Average monthly net salary (after tax)](https://www.numbeo.com/cost-of-living/country_price_rankings?itemId=105) from NUMBEO, an independent, crowdsourced website maintained by a non-governmental individual. *See notebook`coke-index-initial-analysis.ipynb`.*
- For soda consumption data, I got the annual consumption per capita data from [Statista](https://www.statista.com/statistics/505794/cds-per-capita-consumption-in-worlds-top-ten-population-countries/), and world population data from the U.N. *See notebook `soda-consumption-analysis.ipynb`.*
## Methodlogy & Analysis
When measuring the cost of living, organizations such as the the UN or the World Bank deploy a metric called **purchasing power**, which uses **monthly income** calculated from the **gross national income per capita** in relation to cost of goods. But **gross national income per capita**, in my opinion, could not characterize the earning of an average working-class individual.

What I chose to look at instead is the average daily salary (not income), and local coke prices.
#### Variables used for analysis
| Variable | Description | Source |
| ------- | --------- |------|
| Coke price| Sourced from sales prices of 330 ml/12.9 oz bottle size Coca-ola/Pepsi sold in resturants in each country| [NUMBEO](https://www.numbeo.com/cost-of-living/country_price_rankings?itemId=6)|
| daily salary|Average monthly salary divided by 21 (average number of working days in a month)|[NUMBEO]([https://www.numbeo.com/cost-of-living/country_price_rankings?itemId=6](https://www.numbeo.com/cost-of-living/country_price_rankings?itemId=105))|
|Coke per day|Average daily salary divided by the price of Coke in each country||

A scatter plot was used to conduct exploratory analysis on my data:
![Screen Shot 2023-02-05 at 3 27 09 PM](https://user-images.githubusercontent.com/116761432/216843129-f2b92a1b-8617-4e79-aa6f-05043a7fe705.png)



## Findings
## What I learned from this project
## Challenges and possible improvement


 
