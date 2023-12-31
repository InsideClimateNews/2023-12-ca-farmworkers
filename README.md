# Farmworker deaths, temperature, and air pollution in California

### Methodology 

For the review of [federal Occupational Safety and Health Administration](https://www.osha.gov/) OSHA records reported in [this](https://insideclimatenews.org/news/31122023/california-farmworkers-dying-in-the-heat/) Inside Climate News article, we scraped records of farmworker fatalities in California from 2018 to 2022 from OSHA's [accident search](https://www.osha.gov/ords/imis/accidentsearch.html) site.

We also scraped records of employer citations for violations of [California's standard](https://www.dir.ca.gov/title8/3395.html) for heat illness prevention in outdoor places of employment from OSHA's [industry search](https://www.osha.gov/ords/imis/industry.html) site.

For both scrapes, we identified farmworkers and agricultural employers using the following [North American Industry Classification System](https://www.census.gov/programs-surveys/economic-census/year/2022/guidance/understanding-naics.html) (NAICS) codes: `1111`, `1112`, `1113`, `1114`, `1119`, `115`.

For each fatality, we obtained temperature data [for the time and location](https://openweathermap.org/api/one-call-3#history) of the incident (or 12.00 noon local time on that day if no time was recorded), plus records of the maximum temperature [over each of the preceding four days](https://openweathermap.org/api/one-call-3#history_daily_aggregation) using the OpenWeatherMap [One Call API 3.0](https://openweathermap.org/api/one-call-3).

For each fatality, we also obtained records of the 24-hour PM2.5 Air Quality Index recorded by the nearest monitoring station in the federal Environmental Protection Agency's [Air Data](https://www.epa.gov/outdoor-air-quality-data) network for the day of the incident, or the nearest prior day for which data was available.


### Questions/Feedback
Email Peter Aldhous at peter.aldhous@insideclimatenews.org.
