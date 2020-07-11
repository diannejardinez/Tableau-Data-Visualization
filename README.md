# Tableau Visualization - Citi Bike Analytics

**Tableau Public Workbook**: [Citi Bike NYC - 2020 Q1 to Q2 - Summary Report](https://public.tableau.com/profile/diannejardinez#!/vizhome/UCB-CitiBikeNYC-2020Q1Q2-SummaryReport-Final/CitiBikeSummaryReport-2020-Q1Q2)

**Data Source**: [Citi Bike System Data](https://www.citibikenyc.com/system-data)


**Objective**: Aggregate the data in NYC Citi Bike Trip History Logs and design visualizations for each discovered phenomena. The Timespan chosen is January 2020 - June 2020.

---

**ETL**: 
- Extracted data from Citi Bike System Data csv files for January 2020 - June 2020
- Transformed data in Jupyter Notebook:
	- Appended each csv file to a combined dataset
	- Replaced Gender variables of 0, 1, 2 to Unknown, Male, and Female
	- Created and saved this dataset into a csv file
- Loaded dataset into a Tableau Workbook


## Analysis
*To view visualizations and download Tableau Workbook, visit the "Citi Bike NYC - 2020 Q1 to Q2 - Summary Report" link above*

The Summary Report for Citi Bike NYC is sectioned into four parts: Station Popularity, Ridership Growth, User Demographics, and Bike Usage. The purpose of this analysis was to find out who is the Citi Bike clientele.
- Note for dataset: 
	- Customer Type (Customer = 24-hour pass or 3-day pass user; Subscriber = Annual Member)
	- Ages were placed in [Generation Timeline age groups](https://commons.wikimedia.org/wiki/File:Generation_timeline.svg) and the focus was on Baby Boomers (56-74 years), Generation X (40-55 years), Millennials (24-39 years), and Generation Z (8-23 years)
	- Users who use Citi Bike would need to have a smart mobile device and would need to have either downloaded the Citi Bike app or Lyft app

- **Overall**
	- Total number of Trips: 7,508,808
	- Total Trip Duration(seconds): 9,736,719,980
	- Average Trip Duration(minutes): 22
	- Top User by Age Group: Millennials (24-39 years)
	- Top User by Age: 51 years
	- Top User by Gender: Men
	- Top User by Customer Type: Subscriber
	- Top starting Station: West St & Chambers St in Lower Manhattan

- **Station Popularity**
	- Most Popular
		- Most popular stations are located in Manhattan, 51% of stations are located in Manhattan. These places are near establishments such as schools, restaurants, businesses, and the Lincoln Tunnel bridge between New Jersey and New York 
		- Number 1: Station West St & Chambers St in Lower Manhattan
	- Least Popular
		- Least Popular stations are in the Bronx and the center of Central Park in Manhattan. Possibly because these stations are not close to any establishments. One station on Westchester Ave and Jackson Ave is near a MTA Station 
		- Number 1: Station MTL-AOS-5.1 in the middle of Central Park

- **Ridership Growth**
	- Ridership Growth for all stations in gender and age decreased when NYC incorporated their own “Shelter in Place” order, known as [PAUSE](https://ny.curbed.com/2020/3/20/21187022/coronavirus-new-york-shutdown-shelter-in-place), effective April 29, 2020, and increased when the order was [lifted](https://www.nbcnewyork.com/news/local/shutdown-extended-in-nyc-suburbs-5-regions-enter-1st-reopening-phase-friday/2418251/) effective May 15, 2020
	- Ridership participation is higher in Millennials and Men, but growth is difficult to capture during the coronavirus pandemic. Seems that usage possibly illustrates use of Citi Bikes is from an essential worker or for recreation
	- When PAUSE was in effect in April, there was a decrease in growth of -27.3% in women, -42.9% in men, and -4.0% in Unknown gender classification
	- After the PAUSE order was lifted, there was a 140.1% ridership growth in women, 98% in Men, and 168.4% in Unknown gender classification reported in May.
	- Comparing Q1(January - March) to Q2(April - June) there is an increase in Ridership growth in Q2 than Q1

- **User Demographics**
	- User Demographics looked into who(age, gender, and customer type) uses Citi Bikes the longest
	- The longest trip duration were from Millennial Men who subscribe to Citi Bike, when ages were grouped. However the user that has the longest trip duration, when focusing on just age; were customers that did not subscribe to Citi Bike, were 51, and selected Unknown gender classification. This limitation in the data does not offer an accurate representation on Customer Type Demographics by gender

- **Bike Usage: Ridership Peak Hours (Daily and Hourly)**
	- Bike Usage looked into when is the highest Citi Bike usage by weekday and by hour
	- The highest peak by day was different for each age group except for Millennials and Generation Z who both had Sunday as their peak day. Baby Boomers' peak day was Wednesday and Generation X's peak day was Tuesday
	- All age groups had the highest hourly peaks at 5:00 PM, with the second highest hourly peaks at 8:00 AM for Baby Boomers, Generation X, and Millennials and 6:00 PM for Generation Z

- **Bike Usage: Clientele from Popular stations**
	- Bike Usage also looked into the top three stations used for the beginning of the trip and the clientele that use it
	- From the most popular station, West St & Chambers St, the top customer is Millennial Men who subscribe to Citi Bike (when age is grouped)
	- Additionally, this station is located next to a MTA Subway station, World Trade Center, NYC City Hall, Rockefeller Park, and a high amount of restaurants
	

---


![](https://github.com/diannejardinez/Tableau-Data-Visualization/blob/master/Summary-Report-Cover.png)