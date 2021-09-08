
### WTWY Proposal
#### 09/08/2021

#### Question
I have been asked to find the areas in New York City that will allow for maximum face to face engagement with individuals who are passionate
about increasing the participation of women in technology. I plan to build a model which will allow me to find the busiest subway stations at any given time/day, 
and create an informative and easily understandable visualization of that data. 

My client, WomenTechWomenYes will benefit from this. With our additional insight they will be able to engage more people, which will 
result in a greater turnout for their Gala. 

#### Data Description

For this project, I plan to use the MTA turnstile data from the past 3 months. I also believe that adverse weather will 
have a negative impact on transit ridership, resulting in fewer people to engage. Both of these databases are publicly available, and can be cleaned and sorted using SQL. 

Our best individual unit of analysis will be the turnstiles themselves. By examining the volume of passengers going through 
each turnstile at specific times, we will be able to find the busiest stations which will allow for maximum engagement. 

I am unsure of how many street teams are available, so I would like to find the 10 busiest stations in the city.  

#### Tools
I will work with SQLite and SQLALCHEMY to obtain and clean the data. Then I plan on using Python and its Pandas package to gain additional 
insight.Finally, I will use Matplotlib to visualize the data. I am not planning on needing any additional tools at this time. 

#### MVP Goal
My minimum viable product will be a functional program that highlights that some areas are better than others for street teams. 
