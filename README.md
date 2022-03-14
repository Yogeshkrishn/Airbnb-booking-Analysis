# Airbnb-booking-Analysis
Since 2008, guests and hosts have used Airbnb to expand on traveling possibilities and present a more unique, personalized way of experiencing the world. Today, Airbnb became one of a kind service that is used and recognized by the whole world. Data analysis on millions of listings provided through Airbnb is a crucial factor for the company. These millions of listings generate a lot of data - data that can be analyzed and used for security, business decisions, understanding of customers' and providers' (hosts) behavior and performance on the platform, guiding marketing initiatives, implementation of innovative additional services and much more.

This dataset has around 49,000 observations in it with 16 columns and it is a mix between categorical and numeric values.

Explore and analyze the data to discover key understandings (not limited to these) such as :

What can we learn about different hosts and areas?

What can we learn from predictions? (ex: locations, prices, reviews, etc)

Which hosts are the busiest and why?

Is there any noticeable difference of traffic among different areas and what could be the reason for it?

## Problem and Data

We have been provided the listing Data from Airbnb. Whenever a property owner wants to offer their services through Airbnb, they have to list their property and its details. 

If we go through the fields present in the dataset :

**Id**-Unique Id of each property

**name**-Name of properties, which also describes the property

**host_id**-ID of the host, this is unique for all the hosts.

**host_name**- Name of the host , Names may be similar for two hosts.

**neighbourhood_group**-have 5 different regions of New York

**neighbourhood**- these are the subregions of neighbourhood_group , where one neighbourhood belongs to only one neighbourhood group.

**Latitude** contains the coordinates of Latitude for that location.

**Longitude** contains the coordinates of longitude for that location

**room_type** – there are three types of property available,

**price**- price of stay (we have taken it for one night basis)

**minimum_nights**- this is the minimum number of nights for which you have to book a host’s place

**number_of_reviews**-This will be the number of reviews each property has got,we can also use this to infer about the number of customers considering the same customer behaviour across regions.

**last_review**-Date of last review that is posted for the property.

**reviews_per_month**- Number of reviews for each property per month

**calculated_host_listings_count**-Number of listing for each property

**availability_365**-Number of days each property is available out of 365 days of the year

## Steps involved:
**Exploratory Data Analysis :**

After loading the dataset we performed this method by first taking a Snapshot of the whole data.This process helped us figuring out which columns have null values and the datatype of each column. It gave us a better idea of which are key columns on the basis of which we can group our data ,and for which columns will need some cleaning or feature engineering.

**Null values Treatment:**

Our dataset contains some of the null values in Host information and Reviews Data which might tend to disturb our Plots and Aggregation we performed  hence we took their values as 0 for reviews in our project in order to get a better result.

**Making some categorical columns :**

We have converted the minimum night column to a category based feature on normal understanding of time. Reason being ,we wanted to see which region has more number of 1 day booking implying business trips mostly.

**Understanding Correlation among fields:**

Here we have plotted the correlation of fields in a heatmap,which then explains that no two fields are highly correlated; only the number of reviews and reviews per month are correlated with each other and that is (corr=0.55) quite reasonable.



###### Coding Language used-- Python version 3.0 

###### Platform used - Google collab notebooks
