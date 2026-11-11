# Python_Fundamentals_Final
Final Project for Python Fundamentals

https://www.kaggle.com/datasets/sumanbera19/antarctica-climate-dataset-20062025-daily-data

10/23/2026 - Checking for null values using string function "info". No null values in the data, and all columns show a single data type.

10/23/2026 - Checking for duplicate values in the data using string functions "duplicated" and "value_counts". No duplicate values in the data.

10/23/2026 - Checking for standardization of locations, latitudes, and longitudes with "value_counts". All are standardized.

10/23/2026 - Checking for negative wind speeds and precipitations. There are no negative precipitation or wind values.

10/23/2026 - Checking z-scores of temperatures, precipitation, and wind speed for each location to detect outliers. Tested average temperatures, total precipitation, total rain, hours of precipitation, wind speed, and wind gusts for outliers. None detected.

11/06/2026 - Plotted average temperature per location - one line chart per year. Antarctic Peninsula showing average winter temperature increase. South Pole is not the coldest location - East Antarctica location regularly colder despite being further north.
             </p><p>Plotted average daylight hours per day 20-year average with line graph. First converted seconds of daylight to hours of daylight by dividing by 3600. Since 1/1/YYYY should generally have a similar amount of daylight each year, used the means for the same dates (20 values per date). This created a graph with a lot of spikes - difficult to read. Adjusted to 14-day rolling average to even out line graph and make more legible. Weakness - no data for first two weeks of the year. Antarctic Peninsula is the only location to have daylight during deep winter.

11/08/2026 - Created wind roses for each location - color determined by wind strength, r-value determined by frequency. This required converting directional vectors into compass directions. Antarctic Peninsula has two primary wind directions. South Pole has a primary and secondary wind directions. Other three locations showing one primary wind direction.
             </p><p>Plotted precipitation measurements in cm for each location throughout the year - one graph per location. Only one location with significant precipitation - Antarctic Peninsula.

11/10/2026 - Inserted descriptive statistics but narrowed to specific columns - 'temperature_2m_mean', 'temperature_2m_max', 'temperature_2m_min', 'precipitation_sum', 'rain_sum', 'precipitation_hours', 'wind_speed_10m_max', 'wind_gusts_10m_max', 'sunshine_hrs' -- calculated 'sunshine_hrs' from 'sunshine_duration' column by dividing by 3600. Grouped each of these for specific locations.
             </p><p>Added map of Antarctica at beginning of charts with each location plotted - location data viewable on hover.
