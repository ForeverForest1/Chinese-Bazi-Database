**Project 3: Querying the Chinese solar sexagenary calendar**

Background and Problem Statement:
Chinese numerology, or bazi, is a common cultural practice used by many Chinese for date selection and character profiling. Every year, month, day and hour is represented by a pillar, which is combination of a Heavenly Stem (base-10) and the Earthly Branch (base-12) character. The respective pillars can be found in the Chinese solar sexagenary calendar. Every stem and branch represents certain elements, and the interaction of all the elements present at a particular time is used to predict the outcomes of events.

To convert a date from the Gregorian calendar to the Chinese solar sexagenary calendar, a book called Tung Shing (通勝) is used. The Tung Shing also contains description of the suitable activities of the day, which many fengshui practioners and geomancers use.

While there are free websites and apps that provides information for individual dates, the ability to extract multiple dates fulfiling one or more criteria is usually not available, or only found on the paid tier. In this project, we are going to create a digital database containing some basic information of the Tong Shing, which can queried and searched using SQL language.	


Overview of Approach:
We are going to use the scrape information found on Wikibooks (https://en.wikibooks.org/wiki/Ba_Zi).


Results:
The following csvs were created using the information scraped from Wikibooks: 
1. df_birth - 
i. Characters for year, month, day from 1902 to 2048 
ii. Luck pillars - characters, direction and starting age for male and female

2. df_branch - Association of each earthly branch with elements, chinese zodiac, time, hidden stems and the ying-yang qi

3. df_hour - Hour stem character for each combination of day stem and hour branch

4. df_stem - Association of each heavenly stems with elements, organ and the ying-yang qi  

Next Steps:
The csv files will be loaded onto Google BigQuery and queried with SQL language. 