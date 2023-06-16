# Google Data Analytics Capstone: Cyclistic Case Study

## Introduction
Welcome to the Cylistic bike-share analysis case study!
As a junior data analyst of Cyclistic’s marketing analyst team, I analyse historical data of the company in order to identify trends in how their customers use bikes differently. The main tools I use are Microsoft Excel and Tableau.

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

## Data cleaning and manipulation
### Microsoft Excel: initial data cleaning and manipulation
After downloading all 17 files and unzipping them, I housed the files in a temporary folder on my desktop. I also created two subfolders, .CSV files and .XLS files so I have copies of all the original data. Then, I launched Excel, opened each file, and chose to Save As an Excel Workbook file. For each .XLS file, I did the following:


* Removed extra spaces using **TRIM** function
  * Unified formats in **ride_id column** and **rideable_type column**

* Created a column **ride_length**
  * Calculated the length of each ride by subtracting the column **started_at** from the column **ended_at** (example: =D2-C2)
  * Formatted as **custom**
  * Format > Cells > Time > [H]:MM:SS, displaying the accumulated hours the users used since sometimes the bike was rented for more than one day
  * Used the **FILTER and SORT** functions to have a quick screen of the results and discover some errors as some of the started dates and ended dates were typed in in the wrong order. This was correct by sorting the columns by Z to A order and switching the data in the right order
 
* Created a column **day_of_week**
  * Used **WEEKDAY** function to calculate the day of the week that each ride started (example: =WEEKDAY(“started_at”,1))
  * Formatted as a **number** with no decimal
  * Format > Cells > Number (no decimals) > 1,2,3,4,5,6,7
  * Note: 1 = Sunday and 7 = Saturday

### Microsoft Excel: further data manipulation and creating summaries




