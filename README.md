# Weather Insight Dashboard

**1. Project Title: **
Weather Insights Dashboard

**2. Short Description/Purpose: **
An interactive Power BI dashboard that pulls live current-weather, hourly/daily forecast, and air-quality data from the WeatherAPI.com API for five major Pakistani cities (Islamabad, Lahore, Karachi, Murree, Multan). It consolidates each city's feed into unified Current, Forecast (by day/hour), and Master data models, enabling at-a-glance monitoring of temperature, humidity, wind, UV index, precipitation chances, sunrise/sunset times, and air quality indicators (PM2.5, PM10, CO, NO2, O3, SO2) across locations.

**3. Tech Stack: **
- Power BI (Power BI Template / .pbit)
- Power Query (M language) – API ingestion & data shaping
- DAX – measures and calculated tables
- WeatherAPI.com REST API – data source (JSON)
- Data modeling: Relationships established among tables (dates) to enable aggregation.

** 4. Data Source:**
 - WeatherAPI.com (https://www.weatherapi.com/)
- Parameters: 7-day forecast, air quality (aqi=yes) enabled
- Cities queried: Islamabad, Lahore, Karachi, Murree, Multan
- Format: JSON, ingested via Power Query (Web.Contents + Json.Document)
- Refresh: Data is pulled live on report refresh; no scheduled incremental load or historical archiving — each refresh reflects current conditions and the latest 7-day forecast.

**5. Features / Highlights:**
- Multi city coverage — single dashboard tracks 5 main cities side by side
- Current conditions at a glance — temperature (°C/°F), humidity, wind speed/direction, pressure, visibility, UV index
- 7-day forecast — daily min/max/avg temperature, precipitation chance, wind, humidity
- Hourly breakdown — granular hour-by-hour forecast data for detailed planning
- Astronomy data — sunrise, sunset, moonrise/moonset, moon phase per day
- Air quality monitoring — PM2.5, PM10, CO, NO2, O3, SO2
- Consolidated data model — separate per city API pulls combined into unified Master Data, Current Data, Forecast by Day, and Forecast by Hour tables for easy cross-city comparison
- Auto generated date tables — built in calendar tables support time intelligence across all fact tables

**6. Screenshot/Demos:**
Dashboard Preview:(https://github.com/fatimaaafzal20/Weather-Dashboard/blob/main/Weather%20Dashboard.PNG)
