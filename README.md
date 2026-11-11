# Antarctica_Climate_Analysis
Final Project for Python Fundamentals

https://www.kaggle.com/datasets/sumanbera19/antarctica-climate-dataset-20062025-daily-data

10/23/2026 - Checking for null values using string function "info". No null values in the data, and all columns show a single data type.

10/23/2026 - Checking for duplicate values in the data using string functions "duplicated" and "value_counts". No duplicate values in the data.

10/23/2026 - Checking for standardization of locations, latitudes, and longitudes with "value_counts". Any that are not floats would result in errors. All are standardized.

10/23/2026 - Checking for negative wind speeds and precipitations - these cannot be negative and would require changing to positive. There are no negative precipitation or wind values.

10/23/2026 - Checking z-scores of temperatures, precipitation, and wind speed for each location to detect outliers. Tested average temperatures, total precipitation, total rain, hours of precipitation, wind speed, and wind gusts for outliers. None detected.

11/06/2026 - Plotted average temperature per location - one line chart per year once the months and years were extracted from the data. Each month value is a mean of every average temperature recorded that month (Dec 2011 = mean of Dec 1 - Dec 31 averages). Antarctic Peninsula showing average winter temperature increase. South Pole is not the coldest location - East Antarctica location regularly colder despite being further north.
             </p><p>Plotted average daylight hours per day 20-year average with line graph. First converted seconds of daylight to hours of daylight by dividing by 3600. Since 1/1/YYYY should generally have a similar amount of daylight each year, used the means for the same dates (20 values per date). This created a graph with a lot of spikes - difficult to read. Adjusted to 14-day rolling average to even out line graph and make more legible. Weakness - no data for first two weeks of the year. Antarctic Peninsula is the only location to have daylight during deep winter.

11/08/2026 - Created wind roses for each location - color determined by wind strength, r-value determined by frequency. This required converting directional vectors into compass directions. Antarctic Peninsula has two primary wind directions. South Pole has a primary and secondary wind directions. Other three locations showing one primary wind direction. ***WIND ROSES NOT VISIBLE ON GITHUB - ACCESS GOOGLE COLAB - [https://colab.research.google.com/drive/1gAEaStMz5sy4ovCB-DAudyYkzFYcd75u#scrollTo=5bTA1y9HyKuV](https://colab.research.google.com/drive/1gAEaStMz5sy4ovCB-DAudyYkzFYcd75u?usp=sharing)***
             </p><p>Plotted precipitation measurements in cm for each location throughout the year - one graph per location. Only one location with significant precipitation - Antarctic Peninsula.

11/10/2026 - Inserted descriptive statistics but narrowed to specific columns - 'temperature_2m_mean', 'temperature_2m_max', 'temperature_2m_min', 'precipitation_sum', 'rain_sum', 'precipitation_hours', 'wind_speed_10m_max', 'wind_gusts_10m_max', 'sunshine_hrs' -- calculated 'sunshine_hrs' from 'sunshine_duration' column by dividing by 3600. Grouped each of these for specific locations and divided into separate codes - temperature, precipitation, & sunshine.
             </p><p>
             </p><p>Added map of Antarctica at beginning of charts with each location plotted - location data viewable on hover. This required making a dictionary of location names, latitudes, and longitudes. ***MAP NOT VISIBLE ON GITHUB - ACCESS GOOGLE COLAB - [https://colab.research.google.com/drive/1gAEaStMz5sy4ovCB-DAudyYkzFYcd75u#scrollTo=5bTA1y9HyKuV](https://colab.research.google.com/drive/1gAEaStMz5sy4ovCB-DAudyYkzFYcd75u?usp=sharing)***
             </p><p></p><p>Descriptive explanations:
             </p><p>In the descriptive statistics for temperature, the Antarctic Peninsula regularly shows that it is warmer than any other location. Despite being the furthest south location, the South Pole is, on average, warmer than East Antarctica. This is further explored with a visual.
             </p><p>In the descriptive statistics for precipitation, only one location seems to get a significant amount of precipitation - the Antarctic Peninsula. All other locations receive an average of less than 1cm precipitation per year. Because the amount of rain is quite low, it can be inferred that this precipitation tends to be in the form of snow, sleet, or hail.
             </p><p>All wind measurements, in km/hr, were taken at 10m above the ground. Two locations have much lower wind speeds than the others, so it can be inferred that these locations, McMurdo Station and the South Pole, are more sheltered than the others. The other three locations likely have less cover to shield from the wind.
             </p><p>Despite being the furthest location north, the Antarctic Peninsula receives almost half as much daylight throughout the year than the other locations. As demonstrated in the visual below, the other four locations receive significantly more daylight during the summer, even if they don't receive daylight during the winter. It seems that the summer daylight hours contribute quite a bit to the difference.
