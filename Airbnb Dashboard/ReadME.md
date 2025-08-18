# Airbnb NYC Tableau Dashboard  

## Project Overview  
This project explores **Airbnb listings in New York City** using Tableau. The goal is to uncover **pricing patterns** and **demand drivers** across boroughs and neighborhoods, helping understand what factors influence the Airbnb market in NYC.  

The dashboard is built using the **AB_NYC_2019 dataset** and is structured into three main views:  
1. **Introduction** – Context and Airbnb presence in NYC  
2. **General Trends** – What influences price and demand?  
3. **Regional Analysis** – Which areas have higher prices?  

---

## Dataset  
- **File:** `AB_NYC_2019.csv`  
- **Source:** Public Airbnb dataset for New York City (2019)  
- **Key Fields Used:**  
  - `neighbourhood_group` – Borough (Manhattan, Brooklyn, Queens, Bronx, Staten Island)  
  - `neighbourhood` – Detailed neighborhood names  
  - `price` – Price per night (USD)  
  - `number_of_reviews` – Total reviews as a proxy for bookings  
  - `availability_365` – Availability of listing per year  

### Calculated Fields in Tableau  
**Demand Score** – proxy for demand (reviews per available day):  
```tableau
IF [availability_365] > 0 THEN
    ([number_of_reviews] / [availability_365]) * 100
ELSE
    0
END

