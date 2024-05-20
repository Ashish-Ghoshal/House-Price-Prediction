# Predicting House Prices with Apache Spark

## Objective
The objective of this project is to predict the Median house value for the given test data using Apache Spark.

In this, we'll make use of the [California Housing](http://www.dcc.fc.up.pt/~ltorgo/Regression/cal_housing.html) data set. Note, of course, that this is actually 'small' data and that using Spark in this context is mainly to demonstrate a proof of concept.

## Understanding the Data Set

The California Housing data set appeared in a 1997 paper titled *Sparse Spatial Autoregressions*, written by Pace, R. Kelley, and Ronald Barry and published in the Statistics and Probability Letters journal. The researchers built this data set by using the 1990 California census data.

The data contains one row per census block group. A block group is the smallest geographical unit for which the U.S. Census Bureau publishes sample data (a block group typically has a population of 600 to 3,000 people). In this sample, a block group on average includes 1425.5 individuals living in a geographically compact area.

These spatial data contain 20,640 observations on housing prices with 9 economic variables:

<p style="text-align: justify;"></p>
<pre><strong>Longitude:</strong>refers to the angular distance of a geographic place north or south of the earth’s equator for each block group
<strong>Latitude:</strong>refers to the angular distance of a geographic place east or west of the earth’s equator for each block group
<strong>Housing Median Age:</strong>is the median age of the people that belong to a block group. Note that the median is the value that lies at the midpoint of a frequency distribution of observed values
<strong>Total Rooms:</strong>is the total number of rooms in the houses per block group
<strong>Total Bedrooms:</strong>is the total number of bedrooms in the houses per block group
<strong>Population:</strong>is the number of inhabitants of a block group
<strong>Households:</strong>refers to units of houses and their occupants per block group
<strong>Median Income:</strong>is used to register the median income of people who belong to a block group
<strong>Median House Value:</strong>is the dependent variable and refers to the median house value per block group
</pre>

What's more, we also learn that all the block groups have zero entries for the independent and dependent variables have been excluded from the data.

The Median house value is the dependent variable and will be assigned the role of the target variable in our ML model.

Look for houses.zip from [here](http://lib.stat.cmu.edu/datasets/) and download the data.
