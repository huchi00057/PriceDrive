# PriceDrive
Analyzing Used Car Pricing and Regional Trends 

## I. Introduction

Owning a car is essential for living in the US due to its vast size. For international students, getting around can be challenging without a car, often relying on friends or public transportation. Buying a used car offers a feasible solution due to its lower price. However, to choose a suitable used car, factors such as affordability, condition, age, and regional differences must be considered. Differences between states, including climate, terrain, and the urban-rural divide, play significant roles in determining the ideal car for various regions. In summary, understanding the market and considering regional factors is vital for individuals unfamiliar with car ownership in the US.

### A. Explore Topic  
The research focuses on the challenges and considerations in purchasing a used car in the United States, particularly for international students.

### B. Motivation  
The motivation stems from the pivotal role cars play in navigating the vast expanse of the United States. International students, often without access to personal vehicles, face unique transportation obstacles that significantly impact their mobility. By exploring used car ownership, we aim to provide valuable insights to help mitigate these challenges.

### C. Goals  
- Examine the feasibility of purchasing a used car as a solution for international students in the US.
- Identify and analyze the key factors (affordability, condition, age, and regional considerations) influencing the selection of a suitable used car.
- Explore variations in car ownership preferences across states, considering factors like climate, terrain, and urban-rural disparities.
- Provide comprehensive comparisons and guidelines to assist international students in making informed decisions when purchasing a used car in the US.

### D. Explore Questions  
- What are the most popular makes and models of used cars in the dataset, and do their prices vary significantly by region?
- Do regions with high latitude and low temperatures prefer certain brands or types?
- Does the quantity and density of major cities impact the prices of used cars?

---

## II. Methodology

### A. Data Collection  
Two datasets will be used in this study:  
1. **Used Car Dataset**: A dataset from Kaggle titled `final_data.csv` provides detailed information about 27,500 used cars across the United States.  
2. **Climate Dataset**: From the PRISM Climate Group, titled `GlobalLandTemperaturesByState.csv`, containing global land temperatures by state.

#### Table 1: Field Overview of final_data.csv
| Attribute        | Description |
|------------------|-------------|
| id               | A unique identifier for each car listing. |
| region           | The location where the car is listed for sale (e.g., North, South, East). |
| Year             | The year the car was manufactured. |
| Manufacturer     | The manufacturer of the car. |
| condition        | The condition of the car (e.g., excellent, good, fair). |
| cylinders        | The number of cylinders in the car's engine. |
| fuel             | The type of fuel used by the car (e.g., gas, diesel). |
| odometer         | The mileage on the car. |
| title_status     | The status of the car's title (e.g., clean, rebuilt). |
| transmission     | The type of transmission in the car (e.g., manual, automatic). |
| drive            | The type of drive in the car (e.g., fwd, rwd, 4wd). |
| size             | The size category of the car (e.g., compact, mid-size, full-size). |
| type             | The body type of the car (e.g., sedan, SUV, convertible). |
| paint_color      | The color of the car. |
| state            | The state where the car is listed for sale. |
| price            | The listing price of the car. |

#### Table 2: Field Overview of GlobalLandTemperaturesByState.csv
| Attribute                  | Description |
|----------------------------|-------------|
| dt                         | Date of the temperature measurement. |
| AverageTemperature         | The average temperature for the specified date, state, and country. |
| AverageTemperatureUncertainty | Uncertainty of the temperature measurement. |
| State                      | The state where the temperature was recorded. |
| Country                    | The country where the temperature was recorded. |

**Data Preparation:**  
- The dataset will be synchronized by unifying brand categories from 125 to 37 using the Replace function in Excel, correcting issues such as full-width characters and inconsistent capitalization.

### B. Data Preparation
- Synchronize the car brand categories in the dataset to eliminate inconsistencies and ensure consistency for analysis.

### C. Exploratory Data Analysis  
1. **Price and Odometer Distribution**: Both price and odometer histograms show right-skewed distributions, indicating that vehicles with higher prices and higher odometer readings are less frequently listed.  
2. **Most Popular Manufacturers**: Ford, Chevrolet, and BMW are the top sellers.  
3. **Price by Manufacturer**: BMW, Ford, and Chevrolet cars have higher prices, while Honda, Toyota, and Nissan are lower-priced brands, with Japanese brands being about $5,000 cheaper.  
4. **Odometer vs Price**: There is a negative relationship between odometer mileage and price, with cars having lower mileage typically commanding higher prices.  
5. **Price Range**: Ford, Chevrolet, and BMW cars range between $14,000 and $15,000, while Honda, Toyota, and Nissan fall in the $8,000 to $9,000 range. 

---

## III. Findings and Results

### A. Popular Makes of Used Cars and Regional Price Variation  
Ford, Chevrolet, and BMW are the most popular manufacturers. States with higher average car prices tend to prefer luxury cars like BMW, while states with lower average car prices are more likely to purchase domestic brands like Ford. States like Arkansas, which has a lower average car price, show a preference for Volvo.

### B. Preference for Brands in Regions with High Latitude and Low Temperatures  
Regions with significant mountain ranges like Colorado, California, and Washington show a preference for SUVs, as they are ideal for rough terrain. States such as Kentucky, Tennessee, North Carolina, and South Carolina have a high demand for SUVs due to their varied landscapes and outdoor activities.

### C. Impact of City Density on Car Prices  
States with higher city densities, such as California and New York, have higher average car prices. In contrast, states with fewer cities tend to have lower car prices.

---

## IV. Summary

In this project, we explored various factors influencing used car purchases in the United States, with a focus on international students. Key findings include:  
- **Most Popular Brands**: Ford, Chevrolet, and BMW dominate the market, with Japanese brands being cheaper on average.  
- **Price Distribution**: Car prices are right-skewed, with high-price and low-mileage vehicles being less common.  
- **Geographical Analysis**: Terrain, climate, and urban density impact car preferences and prices, with states with more mountains preferring SUVs, and higher city densities correlating with higher car prices.  

This study provides valuable insights for international students and others navigating the complexities of purchasing used cars in the U.S., offering guidance based on region and preferences.
