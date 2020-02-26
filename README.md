# Disney Datasets
These datasets provide information from rides from specific Disney theme parks. In each csv file, the data provided has the date, time, posted wait time, and the actual wait time. I will just be using csv files from rides corresponding to two theme parks: magic kingdom and hollywood studios. The goal is to clean the data once it has been imported, using Python and Pandas. Once the data cleaning has been done, I will import the dataframes to Postgres SQL. The final outlook should be one database in SQL containing two seperate tables.


## Extract
To Extract data from dataset, download the csv files from https://touringplans.com/walt-disney-world/crowd-calendar#DataSets and read them to my jupyter notebook.

## Transform 
Import pandas to create dataframes and start data cleaning process. For the data cleanup, this includes checking for any NaN and negative values, and replacing them with the value of 0. I will need to repeat this process for each individual ride dataframe. As part of the data cleaning process, I will also need to rename column titles.

## Load 
Load dataframes to Postgres SQL. Ensure psycopg2-binary is installed, if not, pip install. Create two separate databases in SQL: "magic_kingdom" which will include two dataframes, and "hollywood_studios" which will include 3 dataframes. Copy and save schemas in jupyter notebook.


# Sources
"7_dwarfs_train.csv", Disney World Ride Wait Time Datasets, TouringPlans.com, June 2018, https://www.touringplans.com/walt-disney-world/crowd-calendar/#DataSets, Accessed February 2020.

"pirates_of_caribbean.csv", Disney World Ride Wait Time Datasets, TouringPlans.com, June 2018, https://www.touringplans.com/walt-disney-world/crowd-calendar/#DataSets, Accessed February 2020.

"rock_n_rollercoaster.csv", Disney World Ride Wait Time Datasets, TouringPlans.com, June 2018, https://www.touringplans.com/walt-disney-world/crowd-calendar/#DataSets, Accessed February 2020.

"toy_story_mania (1).csv", Disney World Ride Wait Time Datasets, TouringPlans.com, June 2018, https://www.touringplans.com/walt-disney-world/crowd-calendar/#DataSets, Accessed February 2020.

"kilimanjaro_safari.csv", Disney World Ride Wait Time Datasets, TouringPlans.com, June 2018, https://www.touringplans.com/walt-disney-world/crowd-calendar/#DataSets, Accessed February 2020.
