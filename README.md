![alt text](PythonLogo.png)

# Python Projects
Here, I am describing some of the python projects that I have done. The projects have been performed inspired by the courses that I took or my personal intersts. 
Four projects are included from which three of them have been completed and I am still working on one of them. 
  * [Bank Stock Market](https://github.com/HamedHeli/PythonProjects/blob/016d47925324a5e1714614c3592f54bab88cb5ab/Bank%20Stock%20Market/Bank%20Stock%20After%20Covid%20.ipynb) (completed): 
      
      In this project, I am comparing the performance of six large US bank stock after the pandemic (from Jan 2020 - Dec 2021) and try to explore how they recovered. After processing data, I have **concluded** that:
 
    * Bank of America, JPMorgan Chase, Goldman Sachs, and Morgan Stanley have similiar performance (correlation > 90%) 
    * Bank of America (BAC) has a solid and low-risk perfomace but its return might not be always maximum; it is an appropriate stock for long-term investors
    * Wells Fargo is also shown to be a good second choice as its perfomance is different with that of Bank of America and causes more diverse portfolio
    * CitiGroup is a good choice for short-time traders: it can provide high gains but it is a high-risk investment and it can also lead to high losses

    **Disclaimer: I am not expert in stock (I atually have little knowledge in the field), the conclusions are not meant to be a robust financial analysis or be taken as financial advice.**
    
    
 * [911 Calls](https://github.com/HamedHeli/PythonProjects/blob/016d47925324a5e1714614c3592f54bab88cb5ab/911%20Calls%20(Capstone%20Project)/911%20Calls%20(Capstone%20Project).ipynb) (completed): 
      
      In this project, I am analyzing 911 call received by Montgomery County, PA, from Dec 2015 - Aug 2016 and try to understnad why and when people are commonly call 911. Here are the **conclusions**:

    * Emergency Medical Services (EMS), Traffic (like car accident), and Fire are respectively the most common reasons people are calling 911. 
    * There is no significant difference between the number of EMS and Fire calls received from a day to day, but Sundays and Saturdays show lower number of Traffic calls.
    * Dec shows relatively lower number of 911 calls compared to other months. 
    * Most of the calls are received from 6:00 AM to 8:00 PM and it is almost indepenet of the month and day.

* [Amazon Web Scaping](https://github.com/HamedHeli/PythonProjects/blob/37792adc18700fac596ed54ea407afd143dd8ef5/Website%20Scraping/Amazon/Amazon%20Scraping.ipynb) (completed): 
    
    In this project, I am presenting a program for deriving the production info from the first seven pages of Amazon after searching a custom keyword. The results include 
    
    * Product Title
    * Price
    * Number of Reviews
    * Review Rating
    * Url address


Cylistic, a bike-share company in Chicago, wants to know who annual members and casual riders are different. They have concluded that members are more profitable for the company and so they want to encourage casual riders to become members. The project description can be found [here](Description.pdf). 

In this case study, I used data to theorize the main difference between how members and casual riders are using the bikes. I was then able to suggest action plan to convert casual riders to annual members. 

### Importing Data
First, we downloaded the data from [link](https://divvy-tripdata.s3.amazonaws.com/index.html). Data include the rider information from July 2013 - Dec 2021. All data are downloded and tranferred into SQL using SSIS and SSMS tools. 

### Data Cleaning
Data are cleaning in SQL ([SQL codes](SQL/SQLQuery.sql)):
  * Mismatched/inconsistent data are replaced so that column data are consistent 
  * Extra spaces and characters are removed from the names
  * Null cells are filled, as much as possible, using the data from other rows
  * Duplicate data are removed
  * Data are checked for integrity and accuracy.

### Data Processing 
Date are processed in Python and initial insights are derived ([Python code](Python/Bike_Sharing.ipynb))

#### Observations:
  * Number of memebrs increase when pandemic started.
  * Memebrs are using bikes more on weekends while casual riders are riding more on weekdays.
  * Trip duration for members is taking longer than casual riders 
  * Common stations for members are cloes to Chicago attractions, cloes to Mishigan Lake, while casual riders use stations distributed across the city
  * Memebrs are slightly younger than casual riders.

#### Hypothesis:
Memebrs are using bikes for leisure activities while casual riders are using bikes for commuting to work.

#### Action Plan:
  * Increasing the number of stations near the Chicago's attractions, especially those around the Mishigan Lake.
  * Providing tandem (twin) bikes which are appropriate for leisure activities. 
  * Seting 20-minute limit for casual riders on weekends, after which the rental fee increases.
  * Equipping bikes with saddles that are more appropriate for women riders.  

### Data Visualization
Date are visualized in Tableau ([Tableau link](https://public.tableau.com/app/profile/hamed7970/viz/GoogleCapstone_16422249161910/Dashboard1))
