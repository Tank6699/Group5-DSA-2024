# Air Quality Index Project Overview
This project leverages OpenAQ, a comprehensive platform that aggregates and shares open air quality data globally, to conduct a detailed analysis of air quality indices (AQI).
## Step 1: Downloading the data:
- Here we downloaded the data set per month for 6 months from 'https://openaq.org'
- Open Aq allows only 30 days at a time
- Time period Jan 2024 to Jul 2024
### Combining the Data:
Once the Data was in the Directory, we combined the Data.
Below is an example of the code used:
      <img width="464" alt="image" src="https://github.com/user-attachments/assets/0045a504-947d-4064-8685-82594355670f">
## Step 2: Importing the Data as Dataframe:
  <img width="349" alt="image" src="https://github.com/user-attachments/assets/4d75ba7c-d124-4333-ba37-929b47729519">
### Viewing the data: 
An example of how the data looks:
    <img width="568" alt="image" src="https://github.com/user-attachments/assets/2e13af1d-63cb-4094-9a4e-3da6505213a8">
#### Variables:
1. **`location_id`**: A unique identifier for the monitoring location. Each city has different location IDs.
2. **`location_name`**: The name or identifier of the monitoring station. This varies between locations in Bucharest, Los Angeles, and Molina de Segura.
3. **`parameter`**: The air quality parameter being measured, such as `pm10` (Particulate Matter 10), `pm2.5` (Particulate Matter 2.5), `no2` (Nitrogen Dioxide), `o3` (Ozone), etc.
4. **`value`**: The recorded measurement of the air quality parameter. This value is provided in the unit specified.
5. **`unit`**: The unit of measurement for the parameter value, such as `µg/m³` (micrograms per cubic meter) for particulate matter or `ppm` (parts per million) for gases.
6. **`datetimeUtc`**: The date and time of the measurement in Coordinated Universal Time (UTC). This timestamp indicates when the data was recorded in UTC.
7. **`datetimeLocal`**: The date and time of the measurement adjusted to the local time zone of the monitoring location. For Bucharest, it is `Europe/Bucharest`; for Los Angeles, it is `America/Los_Angeles`; and for Molina de Segura, it is `Europe/Madrid`.
8. **`timezone`**: The time zone of the monitoring location. This indicates the local time zone where the measurement was taken.
9. **`latitude`**: The latitude coordinate of the monitoring station. This helps in locating the monitoring site geographically.
10. **`longitude`**: The longitude coordinate of the monitoring station. This also helps in locating the monitoring site geographically.
11. **`country_iso`**: The ISO country code for the location of the monitoring station. This column may contain missing values and is often not provided.
12. **`isMobile`**: Indicates whether the monitoring station is mobile. This column may contain missing values in the dataset.
13. **`isMonitor`**: Indicates whether the monitoring station is a fixed monitor. This column may contain missing values in the dataset.
14. **`owner_name`**: The organization responsible for operating the monitoring station. For example, it might be an unknown governmental organization or another entity.
15. **`provider`**: The organization providing the data. For instance, data might be provided by "AirNow," "EEA" (European Environment Agency), or another source.

#### Time Period Covered:
- **Bucharest Data**: The dataset includes measurements from January 4th to June 4th.
- **Los Angeles Data**: The dataset includes measurements from January 4th to June 4th.
- **Molina de Segura Data**: The dataset includes measurements from January 4th to June 4th.
## Step 3: Cleaning the data:
- Converted Datetime to make it easier to use for Daily and Monthly comparisons
    <img width="514" alt="image" src="https://github.com/user-attachments/assets/1e19433a-214f-4eed-8fdc-99ca8e98d443">
#### Subsetting and Grouping 
- Grouping and creating subsets that we will use rather than dropping
  <img width="630" alt="image" src="https://github.com/user-attachments/assets/624279d7-4729-44f1-8943-a4967ac55f8c">
- Additionally Pivot tables were used
    <img width="812" alt="image" src="https://github.com/user-attachments/assets/87e58a6f-c4f7-4255-9e82-2fc994eebd5a">
        <img width="366" alt="image" src="https://github.com/user-attachments/assets/131cc6e5-6ddb-4e49-bf05-1f7e30188db4">
## Step 4: Visualizations
- Using visualization libraries such as matplotlib to





