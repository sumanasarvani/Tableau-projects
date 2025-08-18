# Global Earthquake Dashboard (1900–2013)

## Overview
This dashboard provides a visual analysis of global earthquakes with a magnitude of 6.0 or higher recorded between **1900 and 2013**.  
This dashboard highlights key patterns such as frequency over time, distribution across regions, and relationships between earthquake characteristics.

---

## Features
- **Magnitude Trends Over Time**  
  Displays how the frequency of strong earthquakes has changed across decades.

- **Depth vs Magnitude**  
  Explores the relationship between earthquake depth and magnitude, showing whether deeper quakes are stronger or weaker.

- **Magnitude Distribution**  
  A histogram that highlights the most common magnitudes in the dataset.

- **Magnitude vs RMS**  
  Examines the relationship between recorded magnitude and root mean square (RMS) error, indicating measurement quality.

- **Dmin vs Magnitude**  
  Scatterplot showing the minimum distance from the earthquake epicenter to the nearest seismic station.

- **Top 10 Most Affected Regions**  
  A ranked list of regions with the highest frequency of strong earthquakes.

- **Global Map of Earthquakes**  
  Geographic visualization of earthquake epicenters, clearly highlighting seismic hotspots.

---

## Dataset
- **File:** `Mag6PlusEarthquakes_1900-2013.xlsx`  
- **Columns Used:**
  - `time`: Date of the earthquake  
  - `latitude` & `longitude`: Location of the epicenter  
  - `mag`: Magnitude of the quake  
  - `depth`: Depth (km) at which the earthquake occurred  
  - `rms`: Root Mean Square error for measurement quality  
  - `dmin`: Distance to the nearest seismic station  
  - `place`: Closest named location  

---

## Key Insights
- Earthquakes are highly concentrated along tectonic boundaries, especially the **Pacific Ring of Fire**.  
- Most earthquakes in this dataset fall between **6.0 and 7.0 magnitude**.  
- The number of recorded earthquakes increases over time, partly due to improved monitoring technology.  
- Regions such as **Japan, Fiji, Solomon Islands, and Vanuatu** appear consistently in the top 10 hotspots.  

---

## Tools Used
- **Tableau** for data visualization  
- **Excel / CSV** for raw data storage and preprocessing  

---

## How to Use
1. Open the Tableau dashboard file (`.twb` or `.twbx`).  
2. Interact with filters to explore earthquakes by year, magnitude, and region.  
3. Use the map to zoom in on specific earthquake-prone regions.
