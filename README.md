# Tableau Data Visualization Project

## Authors
**MIST 4610 Section #47114 Group 3**
- [Andrew Bowman](https://www.github.com/andrewbowmn)
- [Kennedy Hankinson](https://www.github.com/kennedyhankinson)
- [Johnny Vo](https://www.github.com/jvjohnny99)
- [Sneha Neelagaru](https://www.github.com/sneelagaru03)
- [Charlie Nelson](https://www.github.com/ugarcn63826)

## Data Set

[Crime Incidents in 2024 dataset](https://catalog.data.gov/dataset/crime-incidents-in-2024)

### Dimensions
- **Rows:** 29,288  
- **Columns:** 24  

### Column Breakdown

>Unique identifiers

| Column             | Data Type | Description                                    |
|--------------------|-----------|------------------------------------------------|
| **CCN**            | string    | Case Control Number (MPD’s unique incident ID) |
| **OBJECTID**       | int64     | ArcGIS object ID                               |
| **OCTO_RECORD_ID** | float64   | Open Data system record ID (all null, excluded from column count)          |



>Date/time fields

| Column         | Data Type | Description                                             |
|----------------|-----------|---------------------------------------------------------|
| **REPORT_DAT** | string    | When the incident was reported (ISO format)             |
| **START_DATE** | string    | Incident start timestamp (ISO with time zone)           |
| **END_DATE**   | string    | Incident end timestamp (ISO with time zone)             |


>Incident attributes

| Column    | Data Type | Description                                  |
|-----------|-----------|----------------------------------------------|
| **SHIFT**   | string    | MPD shift code (e.g. “DAY”, “SWING”, “MID”) |
| **METHOD**  | string    | Method/weapon used (e.g. “GUN”, “KNIFE”)    |
| **OFFENSE** | string    | Offense type (e.g. “ROBBERY”, “ASSAULT”)    |



>Location descriptor

| Column     | Data Type | Description                                                        |
|------------|-----------|--------------------------------------------------------------------|
| **BLOCK**  | string    | Street‐block address (e.g. “1500 BLOCK OF PENNSYLVANIA AVE NW”)     |
| **BID**    | string    | Business Improvement District code (may be blank)                  |



>Planar coordinates

| Column                | Data Type | Description                                           |
|-----------------------|-----------|-------------------------------------------------------|
| **X**, **Y**          | float64   | X & Y Flat-Map Grid Coordinates (2 Columns)                  |
| **XBLOCK**, **YBLOCK**| float64   | X & Y Flat-Map Grid Coordinates of specific block (2 Columns)|


>Geographic identifiers

| Column                    | Data Type | Description                              |
|---------------------------|-----------|------------------------------------------|
| **WARD**                  | float64   | D.C. political ward number               |
| **ANC**                   | string    | Advisory Neighborhood Commission         |
| **DISTRICT**              | float64   | MPD patrol district                      |
| **PSA**                   | float64   | Police Service Area                      |
| **NEIGHBORHOOD_CLUSTER**  | string    | D.C. neighborhood cluster code           |
| **BLOCK_GROUP**           | string    | U.S. Census block group                  |
| **CENSUS_TRACT**          | float64   | U.S. Census tract                        |
| **VOTING_PRECINCT**       | string    | Voting precinct label                    |


>Geographic coordinates

| Column                      | Data Type | Description                    |
|-----------------------------|-----------|--------------------------------|
| **LATITUDE**, **LONGITUDE** | float64   | GPS geographic coordinates (2 Columns)  |
