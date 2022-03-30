# Ford GoBike System Data
## by Jyothirmai Srinathu


## Dataset

> There are 174952 data points in teh data sen after data wrangling! Earler before cleaning the number of data points wer 183412. There are 16 features (duration_sec,start_time,end_time,start_station_id,end_station_id,start_station_name,end_sattion_name,start+_station_latitude and longitude,end_sation_latitude and longitude,bike_id,user_type,member_birth_uyear,member_gender,bike_share_for_all_trip. There are fetures wit hcategories,numeric also.
> When are most trips taken in terms of time of day, day of the week, or month of the year?
> How long does the average trip take?
> Does the above depend on if a user is a subscriber or customer?
I think the start and end_time, duration helps investigating th emost trips taken in a year and also the avergae trip taken and alos user type dependency alos imapcts the above!


## Summary of Findings

> >The max duration of the trip ranges from 250 seconds to 2000 seconds in most cases. Riders are mostly male customers and willing to starts their ride usually around 11pm to 5pm and ends around 6pm. Most busys days are mondays and sundays than other days.Most busy days in the month are after 20th or before 5th of each month. Female customers are willing to ride long trips than others.Surprisingly, no body willing to share rides almost evry body. Interestingly, risers willing to share riding early mornings and late nights. Its may be due to the non availability of the transportation.


## Key Insights for Presentation

> > It was found that the duration variable is too high at one end!For analysis purpose I made log transformation.>Duration_sec has the long distribution 0 to 8000 sec few distribution on the long duration end. When plotted on a log scale, the duratio ndistribution roughly looks unimodal and the peak between 500 and 1000. secs duration The secong highest peak occurs at 500 sec duration and below 500 secs duration ,the third peak occurs.its a right skewed.After 1000 seconds duartion the steep lowrers and find low peak in between 10000 and 20000 duration.I haveny found any unusla variables in categorical varibales like member_gender and user_type data. They were quite normal.

>When looking at the member _birth year it was found that unsual year of birth appears in the data outliers and for safety purpose I have removed those outleirs from the data. Also, the duration_sec for the outliers were above 75% that means above the third quartile range. For safety purpose, I have removed those data points from the original data.