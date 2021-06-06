# Airbnb-NYC

## Installation
The code should run with no issues using Python versions 3.*.

## Source of Data
The data set, containing information about Airbnb descriptions and ratings in New York City, was imported from [Inside Airbnb](http://insideairbnb.com/get-the-data.html) on 2021-05-02. 

## File Descriptions
* one notebook, containing all the codes and explanatory markdown cells,
* one csv file, containing all data needed

## Project Descriptions
### Project Motivation
I tried to understand the most important question of a potential Airbnb host: what should a host do to obtain high ratings from the customers? 

More specifically, I tried to answer the following three questions:
1. Which neighborhood has a high rating in 'location'?
2. Will the ratings be higher, if the host lives in the same neighborhood where the listing is?
3. Overall, what is most important if a host wants to achieve a high overall rating?
### Data Preparation
To answer the above questions, I perform data cleansing to the original data set. Several assumptions are  made, including the following:
* For time-related information, such as the date when the host started, I convert them into day counts until the data scraping day. In other words, I only care about the length of time, instead of specific dates.
* For descriptive information, such as the description of the Airbnb and the "About" of hosts, I avoid doing a text analysis by just counting the lengths of the descriptions. This could be an oversimplification and could be improved in a future work.
* For location-related information, such as the neighbourhoods of Airbnbs and the host locations, I apply some simplifications. For example, for the host locations, I only extract information about whether the host is in New York, instead of caring about the specific locations.

There are other assumptions in my data cleansing process. More can be seen in the notebook, where every assumption is clearly stated by the corresponding code cells.

## Results
The main findings of the code are summarized at [this post](https://medium.com/@joyybai/how-can-an-airbnb-in-nyc-get-high-review-scores-44e48ba44817).

## Licensing
As mentioned above, the data is from Inside Airbnb which is available under a Creative Commons CC0 1.0 Universal (CC0 1.0) "Public Domain Dedication" license. Otherwise, feel free to use the code here as you like!
