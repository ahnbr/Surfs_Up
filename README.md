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



