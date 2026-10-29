# Data

`Airline_Delay.xlsx` is an extract of the **Airline On-Time Statistics and Delay Causes** data published by the US Bureau of Transportation Statistics (BTS):
https://www.transtats.bts.gov/OT_Delay/OT_DelayCause1.asp

- 34,016 rows, 21 columns. One row per carrier, airport and month, January 2024 to June 2025.
- Licence: BTS data is a work of the US Federal Government and is in the public domain. It is redistributed here with credit to BTS. The MIT licence in the repository root applies to the code only.

## Columns

| Column | Type | Description |
|---|---|---|
| year, month | int | Reporting period |
| carrier, carrier_name | text | Airline code and name |
| airport, airport_name | text | Airport code and name |
| arr_flights | float | Arriving flights |
| arr_del15 | float | Arrivals delayed 15 minutes or more |
| carrier_ct, weather_ct, nas_ct, security_ct, late_aircraft_ct | float | Delayed arrivals attributed to each cause |
| arr_cancelled, arr_diverted | float | Cancelled and diverted arrivals |
| arr_delay | float | Total arrival delay minutes |
| carrier_delay, weather_delay, nas_delay, security_delay, late_aircraft_delay | float | Delay minutes attributed to each cause |

To use a fresh download from BTS instead, export the same columns and save it as `data/Airline_Delay.xlsx` (or change the path in the notebook's loading cell).
