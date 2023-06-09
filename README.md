# Airbnb Bookings - Exploratory Data Analysis

<img src = "Images/airbnb_logo.png" width = "500">

## Abstract: 
Business growth of companies begins with a thorough analysis of data. One of the basic tools for data analysis is exploratory data analysis (EDA). The project is the data analysis of Airbnb bookings. The aim of this article is to point out the importance of the EDA in improving the business of companies.


## Acknowledgements

This public dataset is part of Airbnb, and the original source can be found on this website (http://insideairbnb.com)

## 1. Problem Statement
The data generated by users of Airbnb are in millions. Therefore to improve the business the data analysis should focus on both sides of the story, demand (Guests) and supply (Hosts).
* What can we learn about different hosts and areas?
* What can we learn from predictions? (ex: locations, prices, reviews, etc)
* Which hosts are the busiest and why?
* Is there any noticeable difference of traffic among different areas and what could be the reason for it?

## 2. Introduction
Airbnb, Inc. is an American company that operates an online marketplace for lodging, primarily home stays for vacation rentals, and tourism activities. Based in San Francisco, California, the platform is accessible via website and mobile app
Airbnb does not own any of the listed properties; instead, it profits by receiving commission from each booking. The company was founded in 2008 by Brian Chesky, Nathan Blecharczyk and Joe Gebbia. Airbnb is a shortened version of its original name, AirBedandBreakfast.com.
Our goal here is to explore the dataset and draw meaningful insights. It helps in improving the business, by understanding customer preferences.

## 3. Components of EDA
### Data Exploration
It is the first stage of data analysis. Here we can know about the content of the data set and characteristics of the data set. It tells about the size of the data. We can find the missing value of data, detecting outliers, identifying unnecessary fields etc.

### Data Cleaning
Oftentimes the data we load has various faults, such as typo, missing values, incomplete data, etc. By cleaning up, the data will have better quality to be used for further analysis. It involves finding null values, outliers and removing unnecessary fields.

### Data Wrangling
Data wrangling is the process of transforming and mapping data from raw format into another format with the intent of making it more appropriate and valuable for a variety of purposes such as analytics. The goal of data wrangling is to assure quality and useful data.
The most commonly used examples of data wrangling are for:
* Merging several data sources into one data-set for analysis
* Identifying gaps or empty cells in data and either filling or removing them
* Deleting irrelevant or unnecessary data 
* Identifying severe outliers in data and either explaining the inconsistencies or deleting them to facilitate analysis  

### Data Visualization
Data Visualization represents the text or numerical data in a visual format, which makes it easy to grasp the information the data expresses. We, humans, remember the pictures more easily than readable text. Python provides various libraries for data visualization like matplotlib, seaborn, etc.
 
### Applications of EDA
* Transforming Raw data into useful data
* Detect outliers and anomalies (values that are signiﬁcantly different from the other observations)
* Gaining new insights from the data, that can be used to improve the process
* Testing assumptions using EDA 
* Visualize potential relationships between variables

## 4. Steps involved:
 
##### Step1: Importing the necessary Libraries
For the EDA of the given dataset, python libraries like Pandas, Numpy, Matplotlib and Seaborn are used.

##### Step2: Understanding the data
This dataset has around 48,895 observations in it with 16 columns and it is a mix between categorical and numeric values.

##### Step3: Cleaning the Data
Our dataset contains a large number of null values which might tend to disturb our accuracy hence we dropped them at the beginning of our project inorder to get a better result.

##### Step4: Removing unnecessary fields (if any)

##### Step5: Group by & Merge
Using functionality provided by pandas library (like group by, merge etc)  to find the relationships between different variables

##### Step6: Visualizing the outcomes 
using matplotlib and seaborn library

## 5. Exploring Insights from the data

##### What can we learn about different hosts and areas?

Approximately 85% of the hosts are in Manhattan & Brooklyn whereas Staten Is has less than 1% hosts

<img src = "Images/host density.png" width = "400">

##### What can we learn from predictions? (ex: locations, prices, reviews, etc)
 
* Brooklyn and Manhattan are the most reviewed locations.
<img src = "Images/most rvwd - locations.png" width = "700">
  
* Manhattan is the most expensive location whereas Bronx is the cheapest among all.
<img src = "Images/expensive locations.png" width = "500">

* Price v/s Number of Reviews
<img src = "Images/prices vs revws.png" width = "500">

##### Which hosts are the busiest and why?
For the top host category, more Airbnb listings are not resulting in more reviews.
Hosts which have highest listings have average reviews less than the top average reviews in that category

<img src = "Images/busiest hosts.png" width = "1000">

Busiest hosts : (based on top average reviews) <br> 
1- Dona <br>
2- Jj <br>
3- Carol <br>
4- Asa <br>
5- Wanda <br>
Because these hosts :-
Are located in the busiest areas (Manhattan, Brooklyn & Queens) 
Their room type is either Entire home or Private room which is preferred by most people.
Prices are less than 100 (except for one)

##### Is there any noticeable difference of traffic among different areas and what could be the reason for it?
* Brooklyn & Manhattan share approximately 82% of the traffic whereas Staten Is & Bronx are the least popular among the Guests
<img src = "Images/traffic - pie chart.png" width = "400">

* Majority of the Hosts are located in Manhattan & Brooklyn, that's why these areas have the highest traffic
<img src = "Images/host density.png" width = "400">

* Areas having maximum traffic have more number of Private rooms and Entire home/apartment than their counterparts
<img src = "Images/areas - types of room.png" width = "800">

## Conclusion:

* Number of Hosts available in a location affects the traffic - Areas where number of hosts are more have higher reviews or vice-versa
* Majority of Guests prefer to pay a lesser price.
* Types of Room offered affects the traffic (shared room type is the least popular among guests, whereas Private Room is preferred by more than half of the total Guests)
* Areas where the availability of private rooms and entire home/ apartment are maximum, the traffic is more.
* For the top host category, more Airbnb listings are not resulting in more reviews.
 
### References-
* Medium
* Towards Data Science
* Analytics Vidhya
