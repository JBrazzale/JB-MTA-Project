##Finding the Best Subway Stations to Place Street Teams

- Joseph Brazzale


###Abstract

WTWY has enlisted our help to try and discover which subway stations in New York are the busiest. They are 
looking to place street teams to sign people up for a gala, and would like to know the optimal placement of 
these teams. I worked with the publicly available data from the Metropolitan Transit Authority (MTA) to 
discover which stations had the highest volume of riders at a given time of day. After exploring and cleaning 
the data in Pandas, I built a few visualizations to provide an easy-to-read answer. 


###Design
The first step is to scrape the data from the MTA website using the provided script. Then we can import that 
data into Pandas using SQLALCHEMY and get an idea of its structure. The data from the MTA has a few issues due 
to the way that the turnstile counters function. We can "clean" this data using Pandas. Finally, we can take 
that data and generate a few visuals to illustrate our insights. This is done with Matplotlib and Seaborn.


###Data
I decided to look at a three-month window in the spring of 2019. There are a little over 2.6 million data points 
separated into 11 unique columns. The turnstiles keep a cumulative count of all entries and exits, we need to 
look at the daily volume instead. There are also some rows that contain negative numbers, some rows contain very 
large outliers that will skew our data


###Algorithms
1. Group all data by unique turnstile and use aggregation to find the minimum count for that day
    -find the difference between the present day and the previous day to get daily traffic
2. Create a mask that can filter out all of our negative values, and outliers by checking against IQR


###Tools
- SQLITE and SQLALCHEMY for initial exploration
- Pandas to clean our data
- Matplotlib and Seaborn for visualization


###Communication
I will build a PowerPoint and present it to the client. My presentation will display all of my visualizations,
with some brief insights that I have discovered about our data. 
