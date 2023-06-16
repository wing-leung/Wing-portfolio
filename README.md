# Google Data Analytics Capstone: Cyclistic Case Study

## Introduction
Welcome to the Cylistic bike-share analysis case study!
As a junior data analyst of Cyclistic’s marketing analyst team, I analyse historical data of the company in order to identify trends in how their customers use bikes differently. The main tools I use are spreadsheets, SQL and Tableau.

## Scenario
Cyclistic is a fictional bike-share company in Chicago. There are two types of customers using the company’s services: casual riders, customers who purchase single-ride or full-day passes; members, those who purchase annual memberships.
Cyclistic’s financial analysts have concluded that annual members are much more profitable than casual riders. The director of marketing believes that maximising the number of annual memberships is the key for the company’s success.

The marketing analytics team wants to understand the difference in usage of the company’s services between casual riders and annual members. From these insights, the team will develop a new marketing strategy to convert casual riders into annual members. The primary stakeholders for this project include Cyclistic’s director of marketing and the Cyclistic executive team. The Cyclistic marketing analytics team are secondary stakeholders. 

## Defining the problem
The focus of this job is to convert casual riders into Cyclistic annual members through new marketing strategies. To achieve the goal the director has set up three questions for the marketing analyst team to answer through data analysis:

1. How do annual members and casual riders use Cyclistic bikes differently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?

I get assigned to analyse the first question. The focus is to get some insights of the preferences on bike share services of the two groups. This can provide more accurate customer profiles. This will help the marketing analytics team design high quality targeted marketing for converting casual riders into members. For the Cyclistic executive team, these insights will help Cyclistic maximise the number of annual members and will fuel future growth for the company.

**Business Task:**
**To analyse the Cyclistic data set for the year 2020 to understand how annual members and casual riders use Cyclistic bikes differently**

## Data sources:
Cyclistic’s historical trip data from Jan 2022 to May 2023 is used to analyse and identify trends. This can be downloaded from [divvy_tripdata](https://divvy-tripdata.s3.amazonaws.com/index.html) and  has been made available by Motivate International Inc. under this [licence](https://ride.divvybikes.com/data-license-agreement)

It is structured data, organised in rows (records) and columns (fields). There are 13 columns in each file containing data about all rides that took place:

* ride_id               #Ride id - unique
* rideable_type         #Bike type - Classic, Docked, Electric
* started_at            #Trip start day and time
* ended_at              #Trip end day and time
* start_station_name    #Trip start station
* start_station_id      #Trip start station id
* end_station_name      #Trip end station
* end_station_id        #Trip end station id
* start_lat             #Trip start latitude  
* start_lng             #Trip start longitute   
* end_lat               #Trip end latitude  
* end_lat               #Trip end longitute   
* member_casual         #Rider type - Member or Casual
