# surfs_up
Analyzing weather data in Python and SQLite

## Overview of the Analysis
The purpose of this analysis is to analyze temperature data before opening our surf and ice cream shop in Oahu, Hawaii. Our investor, W. Avy, wants us more information about temperature trends for the months of June and December. 

## Results
- The mean temperature in [June](June.png) was 74.94 degrees.
- The mean temperature in [December](December.png) was 71.04 degrees.
- The standard deviation in December, 3.74, was higher than in June, 3.25.

## Summary
The temperature data from June and December shows that the temperatures during these months are good for an ice cream and surf shop. Another query we could run to further analyze these two months would be to look at precipitation for these months over multiple years. For this query we would query Measurement.prcp 'session.query(Measurement.date, Measurement.prcp).filter(extract('month', Measurement.date) == 6).all()'. Similarly, we can extract this data for december as well: session.query(Measurement.date, Measurement.prcp).filter(extract('month', Measurement.date) == 12).all()'.
