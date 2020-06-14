# Boston-Airbnb-Listing-Price-Study
Understand what factors are influencing Airbnb's listing price 
### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Analysis Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

The code should run with no issues using Python 3.

## Analysis Motivation <a name="motivation"></a>

For this project, I was interested in understanding what factors influence Airbnb's listing price at Boston and want to build a simple model to predict the price. Some specific questions I have in mind are:

1. What are the top factors?
2. Which neighbourhoods have the highest listing price? I've lived at Boston for 2 years when pursuing my graduate degree. I am pretty sure certain areas such as Boston Harbour have higher prices than others.
3. Which amenities add the most value to the listing?

## Files Description <a name="files"></a>

There are a notebook in the repo to answer above questions. The approach I took to answer these questions is to start with exploratory visualization and then use a simple regression model to understand the impact of different factors based on coefficients.


## Analysis Results <a name="results"></a>

The findings of the code can also be found [at the post on Medium](https://medium.com/@stacyli0720/boston-airbnb-listing-price-analysis-392ffc2212e2). 

#### What are the top factors that influence listing price?

From the magnitude of coefficient for regression model, we can tell **property type**, **room type**, **neighbourhoor**, **amenities** and **number of bedrooms** are the top predictors. Although strict cancellation policy also shows up as top predictor, it seems to be the result of high price of listing. Hosts need to endure greater loss if expensive listings get cancelled.

It's surprising to me that RVs tend to have a lower price than normal listings and I didn't even know you can rent a boat on Aibrnb.

In terms of amenities, Washer/Dryer is the only one that made it to the top 10 list. Listings with washer/dryer on average are $91 more expensive than the listing without them. Washer/Dryer certainly add value to the listing themselve but I think it's also because washer/dryer are more likely to exist in new apartments or houses, which are usually more expensive.

South Boston Waterfront is the most expensive neighbourhood, followed by Back Bay, Beacon Hill and Bay Village.

Entire home/apt also tends to have a higher price, which makes a lot of sense.

### Which neighbourhoods have the highest listing price?

We can well neighbourhoods near downtown and Boston harbour area have the most expensive listings while city that are farther away from city center such as Rosilindale, West Roxbury and Mattapan have the cheapest listings.

### Which amenities add the most value to the listing?

Top 5 amenities that are adding value to listings are Washer/Dryer, Doorman, AC, WIFI and indoor fireplace. Top 5 amenities with negative effect on the listing prices are Other pets(s), free parking on the street, kitchen, hangers, and free parking on premises. These are an interesting case. Sometimes what a host chooses to list as an amenity is a signal about the "class" of the listing. One example is hanger. We usually just assume every listing has hangers; hosts who choose to list them as a "feature" anyway bring up the shade of not having such a rather basic necessity, which actually signals a lower price.


## Licensing, Authors, and Acknowledgements <a name="licensing"></a>

Must give credit to Inside Airbnb for the data. Link to the [source data] (http://insideairbnb.com/boston/?neighbourhood=&filterEntireHomes=false&filterHighlyAvailable=false&filterRecentReviews=false&filterMultiListings=false) 
