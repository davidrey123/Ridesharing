# Ridesharing Instances 
Benchmark instances for ridesharing or dial-a-ride problems

This repository contains instances for benchmarking ridesharing or dial-a-ride algorithms. Each file contains a list of trips requests with time-window and pickup and dropoff location data.

These instances were synthesized based on observed trips in the city of Melbourne, Australia obtained from the Australian Bureau of Statistics http://www.abs.gov.au/. For each instance a random sample of observed trips was selected. Three instances sizes are provided **small** (S), **medium** (M) and **large** (L):  
S instances correspond to 0.25% of the daily travel demand in Melbourne  
M instances correspond to 0.50% of the daily travel demand in Melbourne   
L instances correspond to 0.75% of the daily travel demand in Melbourne  

Instances are named as follows: "Ridesharing_SIZE_ID.csv" where SIZE is S, M or L and ID is a unique identifier corresponding to a random sample of observed trips of size SIZE. 

The description of the columns in the instances is provided below.

**Column**  Description  
**Announcement**  Trip requests ID
**Origin**  The SLA code of origin  
**Destination** The SLA code of destination  
**Distance_Car-Peak** Distance (km) from origin to destination by car in peak hours  
**Time_Car-Peak**    Time (min) from origin to destination by car in peak hours  
**Announcementtime**    The time when the announcement enters the system  
**Starttime**    Prefered departure time (min), where 0 is 12am  
**Earliesttime**    Earliesst departure time (min), where 0 is 12am    
**Latesttime**    Latest arrival time (min), where 0 is 12am    
**Origin_Latitude**    Latitude of origin point  
**Origin_Longitude**    Longitude of origin point  
**Destination_Latitude**    Latitude of destination point  
**Destination_Longitude**    Longitude of destination point  

These instances were used in the publication _Najmi, Ali, David Rey, and Taha H. Rashidi. "Novel dynamic formulations for real-time ride-sharing systems." Transportation Research Part E: Logistics and Transportation Review 108 (2017): 122-140._ https://doi.org/10.1016/j.tre.2017.10.009. In this paper, trip requests with an ID less than 100,000 are used as **drivers**' announcements whereas remaining trip requests are used as **riders**' announcements.
