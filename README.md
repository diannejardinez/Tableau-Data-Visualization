# Tableau Visualization - Citi Bike Analytics

**Tableau Public Workbook**: [Citi Bike NYC - 2020 Q1 to Q2 - Summary Report](https://public.tableau.com/profile/diannejardinez#!/vizhome/UCB-CitiBikeNYC-2020Q1Q2-SummaryReport-Final/CitiBikeSummaryReport-2020-Q1Q2)


**Data Source**: [Citi Bike System Data](https://www.citibikenyc.com/system-data)


**Objective**: Aggregate the data in NYC Citi Bike Trip History Logs and design visualizations for each discovered phenomena. The Timespan chosen is January 2020 - June 2020.


**ETL**: 
- Extracted data from Citi Bike System Data for January 2020 - June 2020
- Transformed data in Jupyter Notebook:
	- Appended each csv file to a combined dataset
	- Replaced Gender variables of 0, 1, 2 to Unknown, Male, and Female
	- Created and saved this dataset into a csv file
- Loaded dataset into a Tableau Workbook

**Research Questions**:
- How many trips have been recorded total during January 2020 - June 2020?
- By what percentage has ridership grown?
- What are the peak hours in which bikes are used during the weekday? Hourly?
- What are the top and bottom 10 stations in the city for starting a journey?
- What is the gender, age, and customer type breakdown of participants?



## Analysis
*To view visualizations and download Tableau Workbook, visit the "Citi Bike NYC - 2020 Q1 to Q2 - Summary Report" link above*

The Summary Report for Citi Bike NYC is sectioned into four parts: Station Popularity, Ridership Growth, User Demographics, and Bike Usage. **The purpose of this analysis was to find out who is the Citi Bike clientele**.

- Note for dataset: 
	- Customer Type (Customer = 24-hour pass or 3-day pass user; Subscriber = Annual Member)
	- Ages were placed in [Generation Timeline age groups](https://commons.wikimedia.org/wiki/File:Generation_timeline.svg) and the focus was on Baby Boomers (56-74 years), Generation X (40-55 years), Millennials (24-39 years), and Generation Z (8-23 years)


**Citi Bike Clientele Breakdown**
- Who is it?
	- Millennial Man(24-39 years). This group start their bike journey at E 13 St & Avenue A, located in lower Manhattan, near Stuyvesant Town–Peter Cooper Village, also known as StuyTown that contain around 11,250 apartments. They subscribe to Citi Bike. During the weekdays they mostly ride at 8:00 AM and 5:00 PM; during the weekend, they ride the most on Sundays. 


- Other Citi Bike Users
	- Generation X Men (40-55 years old). This group start their bike journey at Pershing Square North, near Grand Central Terminal Station. They subscribe to Citi Bike and ride at 8:00 AM and 5:00 PM, frequently on Tuesdays. 
	- Millennial Woman (24-39 years old). This group start their bike journey at 1 Ave & E 68 St, located in Upper East Side Manhattan. New York-Presbyterian/Weill Cornell Medical Center, Rockefeller University, Rockefeller Research laboratories, and parks are near this station. They subscribe to Citi Bike and ride at 8:00 AM and 5:00 PM, frequently on Sundays. 
	- Generation Z Men (8-23 years old). This group start their bike journey at University Pl & E 8 St, located in lower Manhattan, near New York University(NYU). During the weekdays they mostly ride at 5:00 PM and 6:00 PM and during the weekend, they ride the most on Sundays. 


## Detailed Analysis
- **Overall**
	- Total Number of Trips: 7,508,808
	- Total Trip Duration(seconds): 9,736,719,980
	- Average Trip Duration(minutes): 21
	- Top User by Age Group: Millennials (24-39 years)
	- Top User by Age: 51 years
	- Top User by Gender: Men
	- Top User by Customer Type: Subscriber
	- Top starting Station: West St & Chambers St in Lower Manhattan
	- Top ending Station: 12 Ave & W 40 St on the edge of the Lincoln Tunnel bridge between New Jersey and New York  

- **Station Popularity**
	- Overall most Popular
		- The most popular stations are located in Manhattan. From the dataset, 51% of Citi Bike stations are located in the Manhattan borough. These places are near business establishments such as schools, restaurants, and the Lincoln Tunnel bridge between New Jersey and New York 
		- Number 1: Station West St & Chambers St in Lower Manhattan
		- Popular for Women: 1 Ave & E68 St
		- Popular for Men: Pershing Square North
	- Overall least Popular
		- Least Popular stations are in the Bronx borough and Central Park in Manhattan. Possibly because these stations are not close to any big business establishments 
		- Number 1: Station MTL-AOS-5.1, center of Central Park
		- Least Popular for Women: Wales Ave & E 147
		- Least Popular for Men: MTL-AOS-5.1

- **Ridership Growth**
	- Ridership Growth for all stations in gender and age decreased when New York incorporated their own “Shelter in Place” order, known as [PAUSE](https://ny.curbed.com/2020/3/20/21187022/coronavirus-new-york-shutdown-shelter-in-place), effective April 29, 2020, and increased when the order was [lifted](https://www.nbcnewyork.com/news/local/shutdown-extended-in-nyc-suburbs-5-regions-enter-1st-reopening-phase-friday/2418251/) effective May 15, 2020
	- Ridership participation is higher in men, but growth is difficult to capture during the coronavirus pandemic
	- When PAUSE was in effect in April, there was a decrease in growth of -27.3% in women, -42.9% in men, and -4.0% in Unknown gender classification
	- After the PAUSE order was lifted, there was a 140.1% ridership growth in women, 98% in Men, and 168.4% in Unknown gender classification reported in May
	- Comparing Q1(January - March) to Q2(April - June) there is an increase in Ridership growth in Q2

- **User Demographics**
	- User Demographics looked into who(age, gender, and customer type) uses Citi Bikes the longest
	- The longest trip duration were from Millennial Men who subscribe to Citi Bike, when ages were grouped. However the user that has the longest trip duration, when focusing on just age; were customers that did not subscribe to Citi Bike, were 51, and selected Unknown gender classification. This limitation in the data may not offer an accurate representation on Customer Type Demographics by gender

- **Bike Usage: Ridership Peak Hours (Daily and Hourly)**
	- Bike Usage looked into when is the highest Citi Bike usage by weekday and by hour
	- The highest peak by day was different for each age group except for Millennials and Generation Z who both had Sunday as their peak day. Baby Boomers' peak day was Wednesday and Generation X's peak day was Tuesday
	- All age groups had the highest hourly peaks at 5:00 PM, with the second highest hourly peaks at 8:00 AM for Baby Boomers, Generation X, and Millennials and 6:00 PM for Generation Z

- **Bike Usage: Clientele from Popular stations**
	- Bike Usage also looked into the top ten stations used for the beginning of the trip and the clientele that use it
	- The top customer by Age Group and Gender are Millennial Men with Generation X Men in second
	- Additionally, this station, E 13 St & Avenue A, is located in lower Manhattan which is near Stuyvesant Town–Peter Cooper Village, also known as StuyTown that contain around 11,250 apartments
	- The top customer by Age and Gender are customers who are 51 and selected Unknown as gender
	- It seems that this age has the highest amount of Unknown Gender selection in all top 10 stations. This limitation in data may not offer accurate representation on user Demographics. However, it is good to note that at this age users choose not to disclose their gender.


---


![](https://github.com/diannejardinez/Tableau-Data-Visualization/blob/master/Citi%20Bike%20NYC-Summary%20Report.gif)


---
# Tableau Visualization - Citi Bike Analytics - Instructions

## Background


Congratulations on your new job! As the new lead analyst for the [New York Citi Bike](https://en.wikipedia.org/wiki/Citi_Bike) Program, you are now responsible for overseeing the largest bike sharing program in the United States. In your new role, you will be expected to generate regular reports for city officials looking to publicize and improve the city program.

Since 2013, the Citi Bike Program has implemented a robust infrastructure for collecting data on the program's utilization. Through the team's efforts, each month bike data is collected, organized, and made public on the [Citi Bike Data](https://www.citibikenyc.com/system-data) webpage.

However, while the data has been regularly updated, the team has yet to implement a dashboard or sophisticated reporting process. City officials have a number of questions on the program, so your first task on the job is to build a set of data reports to provide the answers.

## Task

**Your task in this assignment is to aggregate the data found in the Citi Bike Trip History Logs and find two unexpected phenomena.** 

**Design 2-5 visualizations for each discovered phenomena (4-10 total). You may work with a timespan of your choosing. Optionally, you may merge multiple datasets from different periods.** 

**The following are some questions you may wish to tackle. Do not limit yourself to these questions; they are suggestions for a starting point. Be creative!**

* How many trips have been recorded total during the chosen period?

* By what percentage has total ridership grown?

* How has the proportion of short-term customers and annual subscribers changed?

* What are the peak hours in which bikes are used during summer months?

* What are the peak hours in which bikes are used during winter months?

* Today, what are the top 10 stations in the city for starting a journey? (Based on data, why do you hypothesize these are the top locations?)

* Today, what are the top 10 stations in the city for ending a journey? (Based on data, why?)

* Today, what are the bottom 10 stations in the city for starting a journey? (Based on data, why?)

* Today, what are the bottom 10 stations in the city for ending a journey (Based on data, why?)

* Today, what is the gender breakdown of active participants (Male v. Female)?

* How effective has gender outreach been in increasing female ridership over the timespan?

* How does the average trip duration change by age?

* What is the average distance in miles that a bike is ridden?

* Which bikes (by ID) are most likely due for repair or inspection in the timespan?

* How variable is the utilization by bike ID?

**Next, as a chronic over-achiever:**

* Use your visualizations (does not have to be all of them) to design a dashboard for each phenomena.
* The dashboards should be accompanied with an analysis explaining why the phenomena may be occuring. 

**City officials would also like to see one of the following visualizations:**

* **Basic:** A static map that plots all bike stations with a visual indication of the most popular locations to start and end a journey with zip code data overlaid on top.

* **Advanced:** A dynamic map that shows how each station's popularity changes over time (by month and year). Again, with zip code data overlaid on the map.

* The map you choose should also be accompanied by a write-up unveiling any trends that were noticed during your analysis.

**Finally, create your final presentation**

* Create a Tableau story that brings together the visualizations, requested maps, and dashboards.
* This is what will be presented to the officials, so be sure to make it professional, logical, and visually appealing. 

## Considerations

Remember, the people reading your analysis will **NOT** be data analysts. Your audience will be city officials, public administrators, and heads of New York City departments. Your data and analysis needs to be presented in a way that is focused, concise, easy-to-understand, and visually compelling. Your visualizations should be colorful enough to be included in press releases, and your analysis should be thoughtful enough for dictating programmatic changes. 



### Copyright

Data Boot Camp © 2019. All Rights Reserved.

