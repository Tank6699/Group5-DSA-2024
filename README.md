# Analyzing Global Air Quality Index (AQI) Data

## Overview

This project leverages OpenAQ, a comprehensive platform that aggregates and shares open air quality data globally, to conduct a detailed analysis of air quality indices (AQI). The primary goals are to identify trends, compare air quality across different regions, and investigate the impact of certain events (like holidays, wildfires, or policy changes) on air quality. The project uses Python's pandas for data manipulation, matplotlib and seaborn for data visualization, and sklearn for basic predictive modeling.

## Table of Contents
[Data Collection](#data-collection)
[Data Exploration and Analysis](#data-exploration-and-analysis)
[Visualization and Interpretation](#visualization-and-interpretation)
[Dataset](#dataset)
[Contributing](#contributing)
## Data Collection
We use the OpenAQ API to collect AQI data from various cities. The dataset includes key pollutants such as PM2.5, PM10, CO, NO2, SO2, and O3. You can find the API documentation [here](https://docs.openaq.org/).
# Datasets
-All the data sets are found in folder called NewCombined.
-the data sets are downloaded from OPenAq website.
-This data is only from 01 Jan-01 July 2024 only.
-you can "G_5_DSA_project.ipynb " file if you want to access the code we used for our project

# How to Access the Data

**OpenAQ API:** Use the API to filter data by date, location, and pollutant.
**Downloadable Files:** OpenAQ provides periodic data dumps available for download [here](https://openaq.org/#/download).
# Datasets
-All the data sets are found in folder called NewCombined.
-the data sets are downloaded from OPenAq website.
-This data is only from 01 Jan-01 July 2024 only.
-you can "G_5_DSA_project.ipynb " file if you want to access the code we used for our project
# About The Dataset
### Key Features
- **Areas of Coverage:** Data from five stations,Nairobi, Los Angles,Bucharest,Madrid and Rome. and Also we ahve tried to include Nicosia, Suchang_Dong.
- **Pollutants Measured:** PM2.5, PM10, CO, NO2, SO2, O3, and more.
- **Open and Free:** Available for educational and research purposes.

### Access the Data
- **API Access:** Programmatic access to the data via OpenAQ API.
- **Data Dumps:** Periodic data dumps available for download from the OpenAQ website or GitHub.

# Data Exploration and Analysis

Once the data is collected, we perform the following tasks:

-**Data Cleaning:** Handle missing values, duplicate entries, and data types. Convert datetime for daily and monthly comparisons.
-**Data Exploration:** Calculate summary statistics and understand data distribution using histograms, box plots, and scatter plots.
-**Time-Series Analysis:** Analyze AQI trends over time for selected cities.
-**Comparative Analysis:** Compare AQI data across different cities or regions to identify areas with the best and worst air quality.
# Visualization and Interpretation

We create compelling visualizations to represent our findings using matplotlib and seaborn. These include:

- Time series plots showing AQI trends for selected cities.
- Bar charts comparing AQI across different cities.
- Heatmaps visualizing AQI by month.
- Pie charts for parameter distribution and trend graphs.

We then interpret the results and discuss potential reasons behind air quality trends and differences between cities or regions.
## Contributing

We welcome contributions! Please fork the repository and submit a pull request with your changes. Ensure that your code adheres to our coding 
standards and includes appropriate tests.
