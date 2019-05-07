## bot-attacks: Server Bot Attack Visualization

This notebook visualizes bot attacks using an anonymized server log and IP address geolocation.  Bot data is extracted from the log, geolocated with ipinfo, and put in a pandas dataframe.  Bot data is visualized with histograms and a network graphs using the dataframe we built.

For this sample of 72 bots--logged 28 April, 2019--one-third of the bots are from China and Norway.

Moving data between pandas and a postgreSQL database is illustrated as follows.  First, the dataframe is archived to a postgreSQL table called linuxlog.  Next, linuxlog is queried for Singapore.  The results are copied to another dataframe.
***
<br/>**Bot attack geographic locations:**<br/>   
![Alt text](images/geo_map.PNG)
<i/>Note:  If there are multiple IPs in a country, the IP locations are plotted as red circles.  However, countries are only labeled once.<i/>
***
<br/>**A few of the countries linked to their respective bot usernames:**<br/>    
![Alt text](images/country_user_graph.PNG)
***
<br/>**Query postgreSQL table for Singapore:**<br/>

![Alt text](images/postgre_query.PNG)
***
