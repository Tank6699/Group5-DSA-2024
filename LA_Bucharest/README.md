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
- **`location_id`**: A unique identifier for the monitoring location. Each city has different location IDs.
- **`location_name`**: The name or identifier of the monitoring station. This varies between locations in Bucharest, Los Angeles, and Molina de Segura.
- **`parameter`**: The air quality parameter being measured, such as `pm10` (Particulate Matter 10), `pm2.5` (Particulate Matter 2.5), `no2` (Nitrogen Dioxide), `o3` (Ozone), etc.
- **`value`**: The recorded measurement of the air quality parameter. This value is provided in the unit specified.
- **`unit`**: The unit of measurement for the parameter value, such as `µg/m³` (micrograms per cubic meter) for particulate matter or `ppm` (parts per million) for gases.
- **`datetimeUtc`**: The date and time of the measurement in Coordinated Universal Time (UTC). This timestamp indicates when the data was recorded in UTC.
- **`datetimeLocal`**: The date and time of the measurement adjusted to the local time zone of the monitoring location. For Bucharest, it is `Europe/Bucharest`; for Los Angeles, it is `America/Los_Angeles`; and for Molina de Segura, it is `Europe/Madrid`.
- **`timezone`**: The time zone of the monitoring location. This indicates the local time zone where the measurement was taken.
- **`latitude`**: The latitude coordinate of the monitoring station. This helps in locating the monitoring site geographically.
- **`longitude`**: The longitude coordinate of the monitoring station. This also helps in locating the monitoring site geographically.
- **`country_iso`**: The ISO country code for the location of the monitoring station. This column may contain missing values and is often not provided.
- **`isMobile`**: Indicates whether the monitoring station is mobile. This column may contain missing values in the dataset.
- **`isMonitor`**: Indicates whether the monitoring station is a fixed monitor. This column may contain missing values in the dataset.
- **`owner_name`**: The organization responsible for operating the monitoring station. For example, it might be an unknown governmental organization or another entity.
- **`provider`**: The organization providing the data. For instance, data might be provided by "AirNow," "EEA" (European Environment Agency), or another source.

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
- Using visualization libraries such as matplotlib and seaborn to plot appropriate graphs
- An example to plot a graph of 24 hour averaged Pollutant level is below:
        <img width="740" alt="image" src="https://github.com/user-attachments/assets/068b6d23-ed39-4c65-a11f-6e20225d1aac">
- An example of Pie chart to check distribution of Parameters:
        <img width="826" alt="image" src="https://github.com/user-attachments/assets/b9f670ef-b5c3-4699-992f-054f8f1f5d8f">
        ![image](https://github.com/user-attachments/assets/1608e782-c2dd-4ed6-af51-09bdb2e09d86)
- An example of 6 month Trend:
        <img width="826" alt="image" src="https://github.com/user-attachments/assets/c25ae487-7601-4d07-814c-1a5e6c226d5d">
        ![image](https://github.com/user-attachments/assets/dc0313b1-5aff-43fd-9b2b-0bde9ace382f)
- An Example of Air Qualit Index:
        <img width="858" alt="image" src="https://github.com/user-attachments/assets/ad73907f-b41e-4398-91c6-23c420907fa4">
        ![image](https://github.com/user-attachments/assets/aded56a5-2956-4724-b252-2c7d4ec3d113)
- An Example of AQI Distribution:
        <img width="778" alt="image" src="https://github.com/user-attachments/assets/6d8ec22c-9975-4a1a-85c9-3d930be56e6f">
        ![image](https://github.com/user-attachments/assets/0923f843-f7a0-46c2-aacc-169f3c7570cc)
## Step 5: Analysis of the Daata and Visualizations:
- Examples of side by side analysis of the different visualizations:
<img width="867" alt="image" src="https://github.com/user-attachments/assets/c293805b-c3f4-4a18-b004-a173d6507682">
<img width="884" alt="image" src="https://github.com/user-attachments/assets/b8a18f06-40b7-40c2-a6f6-dea3e1e5b9af">
- Some possible explanations of the Data were then deduced:
  <img width="896" alt="image" src="https://github.com/user-attachments/assets/b3a20a9e-f6ce-4e3e-a36e-b76494b9935d">
## Step 6: Comparison between the Different countries
## Step 7: Summary of our findings
## Step 8: Conclusion

      











