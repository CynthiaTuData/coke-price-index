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

What I chose to look at instead is the average daily salary, and local coke prices.
#### Variables used for analysis
| Variable | Description | Source |
| ------- | --------- |------|
| Coke price| Sourced from sales prices of 330 ml/12.9 oz bottle size Coca-ola/Pepsi sold in resturants in each country| [NUMBEO](https://www.numbeo.com/cost-of-living/country_price_rankings?itemId=6)|
| daily salary|Average monthly salary divided by 21 (average number of working days in a month)|[NUMBEO]([https://www.numbeo.com/cost-of-living/country_price_rankings?itemId=6](https://www.numbeo.com/cost-of-living/country_price_rankings?itemId=105))|
|Coke per day|Average daily salary divided by the price of Coke in each country||

## Findings

I used scatterplot and map to conduct exploratory analysis on my data:
![Screen Shot 2023-02-05 at 3 27 09 PM](https://user-images.githubusercontent.com/116761432/216843129-f2b92a1b-8617-4e79-aa6f-05043a7fe705.png)
As seen here, the distribution of Coke prices is roughly in relation with the country's income level. Generally, the higher the salary, the more expensive the Cokes sold in that country. There aren't any countries with relatively high Coke prices with lower pay. 

![Screen Shot 2023-02-04 at 6 59 47 PM](https://user-images.githubusercontent.com/116761432/216844785-e01e8673-3585-4c68-be16-82d33c2d2a14.png)
By putting data on the map, we are able to get the geographic information of Coke affordability. The places where Coke is most affordable are countries where Coke prices are very low while salary level is above average. These are Middle Eastern countries such as Kuwait and Qatar. The least affordable countries to buy Coke are in Africa and South America.
*See my [story](https://xinyitu.github.io/coke-index/) for the interactive version of the map.*

## What I learned from this project
For this project, data collection and analysis is fairly easy to execute. 

What challenged me the most is deciding what data to use (salary or income, median or average, wholesale prices or resturant prices, etc.). Due to the nature of this project, I wan not able to find any official source documenting Coke prices in the world. Therefore, I had to choose quantity over quality and picked the source with more available data.

Visualizing data posted another challenge. The data I want to highlight happen to be a cluster of smaller countries that are almost invisible when looking at the world map. For that, I used annotation on the map version of my visualization, and create a tabular version to display the data.

## Challenges and possible improvement
- Coke prices and salary data might be inaccurate due to how the data source collects and processes the data.
- Coke prices and salary may fluctuate.
- Ideally, I would use median salary instead of average salary in order to accurately reflect earnings. But median salary data is difficult to find on the net when I work on this project.
- Data is some countries are missing. One way to improve this is scraping Coke prices in resturants where data is missing, using Google Maps or Yelp.
- Coke affordibility is only a **fun way** to understand the cost of living, since the price of Coke is influenced by many other factors. For example, tax policies on beverages would impact Coke prices. The cost of distribution and bottling in different countries also differs. Coke demand and supply is another huge factor when deciding sale prices.

## Contact
I can be reached at xt2274@columbia.edu or on Twitter @CynthiaTu2. My inbox is open for any comments, suggestions, angry email telling me what I did wrong in this project... Feel free to let me know what's your favorite Coke flavor/Coca-cola product! Mine is Vanilla Coke and an Orange drink name "Qoo" (酷儿).

![qoo-drink](https://user-images.githubusercontent.com/116761432/216846234-7a9c832d-36ff-42df-af7e-8d534cb09021.jpg)
