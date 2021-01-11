# Surfs_Up

# Purpose of Analysis
We were given the task to analyze the temperatures for June and December in order to consider the viability of opening a surf and ice cream shop in Hawaii. 

# Approach
- By utilizing the extract function, we were able to isolate the pertinent temperature data for the months of June and December between the years 2000-2017.

- Month of June:
june_tobs = session.query(Measurement.date, Measurement.tobs).filter(extract('month', Measurement.date) == 6).all()

- Month of December:
december_tobs = session.query(Measurement.date, Measurement.tobs).filter(extract('month', Measurement.date) == 12).all()

After that, we looked at the statistical average and fluctuation (standard deviation) as well as the high and lows of the temperature for the given months we were looking at. This was done in order to determine how sustainable this shop would be given the shop would be a tourist-centric endeadvor. 

# Results

## June
<img width="133" alt="Screen Shot 2021-01-11 at 1 50 46 PM" src="https://user-images.githubusercontent.com/68168883/104226123-4c889d00-5415-11eb-9a9f-2a59c1a7f68e.png">

## December 
<img width="158" alt="Screen Shot 2021-01-11 at 2 01 49 PM" src="https://user-images.githubusercontent.com/68168883/104226369-adb07080-5415-11eb-8f62-49264400f792.png">

We can see from the comparison of the 2, that June on average was warmer than December, as one would expect. The high temperature for June was warmer than December and the low temperature for December was lower than June. The difference in the standard deviation for the temperatures for June and December were very close (a difference of 0.5) indicating that over this period of time, there was not a great deal of temperature fluctuation. 

# Summary

- From this analysis, we can surmise that it might get a little chillier in the evening in December but that temperature (56 degrees) would still likely be warmer and more appealing for those living in colder places (like New York!). With the average temperature still at 71 degrees, it would indicate that this would be a desirable destination for those trying to escape the cold weather. 

- An added bonus is that even in the summer months, it doesn't appear as though the high temperature or average temperature is oppressively hot. This is important because that would allow Hawaii to still be a desirable vacation locale even during the warmer summer months. What this would indicate is that because of the relatively steady weather, Hawaii would remain a place to attract tourists year round. 

- Some other important data that we should consider would be factors such as rainfall and humidity to go along with the temperature. This would give us a more well-rounded view of the overall climate in Hawaii during the months of June and December. Additional information regarding the temperature of the months between June and December would also provide more information for us to glean from in order to gain a better understanding of the overall viability of this business venture. 
