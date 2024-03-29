# Predicting Changes in the Seattle Housing Market

## Project Description
Our project will focus on determining whether or not we can accurately predict changes in the Seattle housing market based on a set of variables such as the percentage of houses increasing in value and changes in Zillow- estimated sale prices. We have decided to use the median home sale price as our outcome for seeing changes in the overall housing market. When the median home sale price is higher, this represents changes in the entire market as a whole. The first step is to determine the relationship between these variables and our outcome of interest, our median sale price. Once we have established these relationships, the second task is to see if we can use those relationships to predict changes in the housing market possibly weeks ahead. 

The significance of what we are trying to achieve is clear; everybody from everyday prospective home buyers to large real estate conglomerates would find it useful to be able to predict changes in the market, and figuring out when the “optimal” times of the year are for purchasing real estate. The target audience would be groups of people who are planning to buy or sell houses in a few months or years, for own use or for financial investment. The area we are focusing on is the Seattle area, and thus, people who plan to move here, as an average buyer, might be interested in our study. In addition, house selling or investing relevant companies like Zillow might be interested in our study as well. The audience would be able to learn the trend of median housing prices in Seattle area, what some of the areas would be the best to move to or investigate in, which months are the best time to buy or sell the properties, how to pick houses that have greater growth potential, etc. 

The ceiling of what can be discovered cannot be understated; in a published article discussing possible explanations for spikes in prices, the researchers found that when house prices increase significantly faster than wages, houses become less affordable. This not only affects house buyers, but also renters and people living in social housing. This price increase also leads to a huge increase in first time buyers’ mortgage repayments. In turn, any research of predicting future house prices could help determine if there would be an upcoming housing affordability problem for the city. (PM)

Predicting home values is no new topic to the world of regression and machine learning, with many websites suggesting predictors such as “supply and demand, interest rates, economic growth, demographics, location, the potential of growth, a second bedroom, parking, and home improvements”, among others (House Prices). This raises possible factors and covariates when we discuss what affects housing prices. While it is possible to exclusively look at real estate metrics, the greater state of the economy should also be considered when trying to find relationships between the housing prices and the surrounding environment for those changes. Possible relationships are explored further in an academic paper published discussing the most prominent explanatory variables in a study of London. According to this paper that focuses on finding the factors that influence the real estate price in London, several of the most significant variables that may affect house price including population density, income, and GVA (the measure of the value of goods and services in that area) (Gu).

In terms of what we are testing, we are answering the question of whether there is a significant relationship between the median home sale price of an area, and the population of that area, percent of houses increasing in value, Median Home Value and Average Number of Days of Homes on Zillow. We will be mainly working with the Zillow Research Dataset, which is provided by Zillow itself. The dataset includes spreadsheets of different housing relevant metrics, which can be obtained by state, metro, county, city or zip code. If necessary, we may try to use several other metrics from population housing dataset found from the Data.WA.gov website, this dataset includes population and housing information for Washington state for 2000 and 2010. Since there are multiple variables that we want to take into consideration, we might use the multivariate linear regression model to filter out the most relevant variables to housing price. In terms of machine learning methods for using our data to predict changes in the market, we may use regression models instead of classifier models, since we are not predicting categories. For example, we may try to use the KNN tree or decision tree.

## Technical Description

For the output of our results, we plan on using an ipython page in markdown to compile an HTML style webpage. In terms of possible management and future scope issues, for starters, there may be lots of missing data points within the dataset, which we need to handle. Possibly transitioning the scope from just the Seattle area to a statewide, possibly even a nationwide focus will also raise problems in “normalizing” differing economies (a $400,000 house in Cleveland looks a lot different from a $400,000 house in Seattle). We also may need to explore new models for the prediction in order to get more accurate results. For instance, the gradient boosting model seems to be a suitable one for price prediction, but we need to do more research to figure out how to train and implement it. In addition, as we may need to look for new techniques that are specifically used for predicting price. We also need to figure out a way to handle the large amounts of data available on the Zillow API without necessarily downloading millions of pieces of data at a time.

In terms of our initial procedure of analysis, we plan on first doing some data clean up and preparation, such as properly handling the missing values in the dataset and creating new variables based on the existed variables. Then we might make some visualizations on certain variables to see the trend, but we would ultimately use sklearn feature selection (univariate feature selection, etc.) to identify the most relevant variables. After that, we would start to machine learning modeling, possible modeling algorithms we might try to use are KNN tree and gradient boosting. We would split the testing and training data first, and then perform cross-validation and grid-research; scalers would be added depending on the situation. When we are finished training the models, we would use those models to do the prediction. 

When looking ahead at possible problems in our analysis process, since the housing prices could be greatly influenced by supply and demand, we would have to have some sort of method to account for any relevant supply-demand variables. For example, when a city has strong economic growth and job creation, housing prices will increase. More jobs bring new residents to the city which increases the demand for housing and in result increases the price of houses. Another possible issue can arise when we look at two sources of data, and have to figure out a way to combine them.

## References
“Why West Coast home prices are surging” -Kathryn Vasel https://money.cnn.com/2018/06/13/real_estate/west-coast-housing-markets/index.html

“Why are House Prices so High?” -Positive Money
https://positivemoney.org/issues/house-prices/

“House Prices.” Information About Factors That Determine Property Prices - HomeGuru, www.homeguru.com.au/house-prices.

Gu Yiyang, “What are the most important factors that influence the changes in London Real Estate Prices? How to quantify them?”,  https://arxiv.org/pdf/1802.08238.pdf









