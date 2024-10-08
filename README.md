# Anomaly-Detection-with-EarthObservation
This repository is the result of an academic course assignment focused on detecting sea surface temperature anomalies using MODIS satellite data. The project includes the calculation of the ENSO index to identify El Niño and La Niña events.

## Outputs
###  El Niño and La Niña explanation

![Methodological Flowchart](0_Media/0_elnino-lanina_explanation.jpg)

El Nino Southern Oscillation (ENSO) is the most important year-to-year climate signal on Earth. It is a part of the climate system that is marked by warm El Nino(McPhaden et al., 2006), unusually high sea surface temperatures in the tropical Pacific Ocean's central and eastern regions and by widespread shifts in the region's surface pressure and cold La Nia events (Glantz et al., 2018). Scientists from around the world were unable to determine the cause of ENSO events; however, they developed indexes to anticipate and monitor these occurrences (Hafez, 2016). For this Assignment, I have used Oceanic Nino Index (ONI) which is based on fluctuations in 3-month running means (3-MRMs) of sea surface temperatures (SSTs) in Nino 3.4 region, a region of the central Pacific (Glantz & Ramirez, 2020).

---

### Methodological Flowchart

![Methodological Flowchart](0_Media/2_Methodological_Flowchart.png)

#### **Step 1: Initialization and Data Access**
- **Initialization GEE and Authentication:** 
  - Set up Google Earth Engine (GEE) by authenticating and initializing the session to access the GEE platform.
- **Data Access from GEE:** 
  - Retrieve the required data from GEE for further analysis.
- **Data Filtering for specific band and year:** 
  - Apply filters to focus on a specific band (such as temperature or precipitation) and a particular year or set of years.

#### **Step 2: Computing Monthly Mean**
- **Computing Monthly Mean:** 
  - Calculate the average values for the selected data on a monthly basis.
- **Creating Geometry and Time Series of Monthly Mean:** 
  - Define the geographic area of interest and create a time series based on the monthly mean data for analysis.

#### **Step 3: Computing Climatology**
- **Computing Monthly Climatology and Standard Deviation:** 
  - Calculate the long-term monthly average (climatology) and the standard deviation to understand the variability across months.
- **Creating Time Series of Monthly Climatology:** 
  - Generate a time series that shows the monthly climatological averages over time.

#### **Step 4: Calculating Anomalies and Observing Trends**
- **Calculating Anomalies:** 
  - Compute the difference between observed values and the climatology to identify anomalies, which show deviations from normal conditions.
- **Anomaly Smoothing with 3-monthly Running Mean:** 
  - Apply a 3-month running mean to smooth out the anomalies, reducing noise and making trends clearer.
- **Plotting and Observing El Niño and La Niña Trend:** 
  - Visualize the data to observe patterns related to El Niño and La Niña, which are significant climate phenomena affecting global weather patterns.


---

### Step wise Outputs

![Methodological Flowchart](0_Media/3_StepWiseOutputs.png)

---

### Final Output

![Methodological Flowchart](0_Media/4_Final_Output.png)
