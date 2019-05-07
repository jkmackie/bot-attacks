## bot-attacks: Authorization Log Notebook

***
This notebook visualizes bot (Invalid user) attacks using an anonymized server log and IP address geolocation.  Bot
data is extracted from the log, geolocated with ipinfo, and put in a pandas dataframe.  Bot data is visualized
using histograms and a network graphs.  

Dataframe is archived to postgreSQL table linuxlog.  linuxlog is queried for Singapore and results saved to
singapore_df dataframe.
***
