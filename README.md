# House Rocket Project - Insights
# Business Problem:
House Rocket is a fictional company, that buys and sells houses in Seattle.
The main goal of the company is to buy good houses with good prices and sell them for higher prices later.
The company doesn’t have a method to decide wich houses should be bought, and doesn`t have a pricing system to set the sales prices of the houses.

# Business Assumptions:
- The company hasn’t defined a maximum number of houses it wants to buy.
- In addition to buying and selling houses, the company also considers buying houses that need to be renovated.

# Business Strategy:
- **Step 01. Data collect:** The data was collected in the Kaggle platform, as a csv file and downloaded. The file contains data from houses in Seattle. The data analysis was made using Python.
- **Step 02. Data Statistics:** statistic data were calculated in order to identify outliers and errors.
- **Step 03. Data Cleansing:** data that were considered miswritten errors were removed.
- **Step 04. Insights:** The data attributes were analyzed in order to identify relevant information for the business.
- **Step 05. Identify good houses to buy:** Two groups of houses were identified as great houses to buy to make profitable results for the company.
- **Step 06. Pricing:** A system to set a price was created for both groups of houses.
- **Step 07. Results:** An app was developed to show the two lists of houses, their attributes, sales price, renovation price and profit.

# Insights: 
**Hypothesis 1:** Houses that have nice views are, on average, at least 100% more expensive than the ones that don`t have nice views.

**True:** Houses that have nice views are, on average, 125% more expensive than the ones that don`t have nice views.

**Hypothesis 2:** Houses that were built after 1990 are, on average, at least 15% more expensive than the ones that were built before this year.

**True:** Houses that were built after 1990 are, on average, 19,5% more expensive than the ones that were built before this year.

**Hypothesis 3:** Houses that were renovated after 1990 are, on average, at least 50% more expensive than the ones that were not renovated after 1990.

**True:** Houses that were renovated after 1990 are, on average, 54% more expensive than the ones that were not renovated after 1990.

**Hypothesis 4:** Houses that have nice views, that were built or renovated after 1990 and that are in great conditions are, on average, at least 20% more expensive than houses that also have nice views but were built before 1990, were not renovated since then, and are not in great conditions.

**True:** Houses that have nice views, that were built or renovated after 1990 and that are in great conditions are, on average, 21,46% more expensive than houses that also have nice views but were built before 1990, were not renovated since then, and are not in great conditions.   

# Houses to buy - group 1
- After the business insights, two groups of houses were identified as great houses to buy to make profitable results for the company.
- The first group of houses to buy contains houses in great conditions and good prices.
- In order to compose this group, the data was divided in subgroups of houses that have the same number of bedrooms and are placed in the same region.
- For each subgroup, the median price was calculated. Houses that have its price below median and are in great conditions were added to the list of Houses to Buy. 
- The sale price was defined as the median price from each subgroup, that is composed by houses with the same number of bedrooms and placed in the same region. For example, the sale price of houses with 4 bedrooms and with the zipcode 98126 have the sale price $ 459000, that is the median price of houses in this group.
- The total number of houses in this group is 753.

# Houses to buy - group 2
- The second group of houses to buy contains houses that have nice views, were built BEFORE 1990, were NOT renovated since then, and are NOT in great conditions.
- These houses were considered potential houses to be renovated and sold after that.
- The sale price of these houses considered an increase of 21% of its purchase price. This number is the price difference from these houses to the ones that also have nice views, were built or renovated AFTER 1990 and ARE in great conditions. It has been calculated in 'Hipothesys' 4 from  the 'Insights' section.
- An amount of money of 10% of the purchase price of the houses was destinated to renovate the houses. 
- The sale price is the median price from each subgroup, that is composed by houses with the same number of bedrooms and placed in the same region.
- The number of houses in this group is 445.

# Compiled Results
In the table below you can see the summary of the expected results for each one of the groups:
| Group          | Number of Houses | Average Price | Average Sale Price | renovation cost| total profit  |
|:-------------- |:-----------------|:--------------|:-------------------|:---------------|:--------------|
| Houses Group 1 |        752       |   426594.61   |     511717.95	     |     0          |  64012756.00  |
| Houses Group 2 |        445       |   959168.86   |     1160594.32     |     95916.89   |  46951315.73  |
|                |                  |               |                    |                |  110964071.73 | 

# App with results
The following app was created to visualize the list of houses that were suggested for the company to buy. 

The app has both lists 'Houses to Buy - group 1' and 'Houses to Buy - Group 2' and some filters for a better experience.

https://houses-what-to-buy.herokuapp.com/





