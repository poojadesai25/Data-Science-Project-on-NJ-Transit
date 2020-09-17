# Data-Science-Project-on-NJ-Transit

# Project Overview
The Project is aimed to explore, analyse and realise the delays in the NJ-Transit travel route and the effect of delay/cancellation of NJ-Transit line on the daily commuters.
NJT, is a state-owned public transportation system that serves the US state of New Jersey, along with portions of New York State and Pennsylvania.
The data is of 9 years and contains information about both NJ Transit and Amtrak (Northeast Corridor) train trips. In later stages, Amtrack has been discarded and all the operations are performed on NJ Transit data.
The data includes stop-level, minute resolution data on 287,000+ train trips (248,000+ NJ Transit trips, 38,000+ Amtrak trips). But we are strictly focusing on NJ Transit trips. The data is released by the government.

Column names include:

Column Name| Description
|----------|------------|
Date| Date of operation according to the 27-hour NJ Transit schedule
train_id| These are unique on a daily and correspond to the same scheduled train                      
stop_sequence| Scheduled stop number for the stop in the row
from| Station the train is traveling from for the stop in the current row
from_id| Station id for the "from" station
to| Station the train is arriving to for the stop in the current row
to_id| Station id for the "to" station. 
scheduled_time| the scheduled departure time out of the "to" stop
actual_time| If "departed", then actual departure time out of the "to" stop
actual_time| If "cancelled", the time at which this stop was cancelled 
           | If "estimated", the estimated departure time out of the "to" stop
delay_minutes| The difference between actual_time and scheduled_time, in minutes
Status| Can take the values "departed", "cancelled", or "estimated"
line| The train line on NJ Transit or Amtrak
