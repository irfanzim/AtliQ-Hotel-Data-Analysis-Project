# AtliQ-Hotel-Data-Analysis-Project

## **Project Overview:**

- **Objective:** Address challenges faced by Atliq Grands, a leading Indian hotel chain, including increasing competition and declining revenue.
- **Goal:** Use data analysis to provide actionable insights to improve customer retention and drive revenue growth.

## **Datasets Overview**
The project uses a combination of dimensional and fact tables:

- **dim_date.csv:** Date information with fields such as date, month, week and date type (weekday/weekend).
- **dim_hotels.csv:** List of hotels with their respective IDs, names, category and city.
- **dim_rooms.csv:** Room details including room category and type.
- **fact_aggregated_bookings.csv:** Aggregated booking data with property id, total bookings, capacity etc.
- **fact_bookings.csv:** Detailed booking transactions with information on guests, room categories, booking dates, revenue etc.

## **Highlights of the Project**
**1. Data Exploration**
- Importing Libraries:
  - Used Pandas for data manipulation and Matplotlib for visualization.
- Loading Datasets:
  -  Loaded the datasets using Pandas to begin initial analysis.
  -  Displayed the first few rows to understand the data structure.
- Initial Data Inspection:
  - Explored shape, unique columns, booking status, quick statistics etc. to get an overview of available datasets.

**2. Data Cleaning**
- Handling Missing Values:
  - Identified missing values across all datasets using isnull().sum().
  - Filled or removed missing values based on data significance.
- Handling Inconsistencies:
  - Removed rows where successful_bookings exceeded capacity.
  - Converted negative values to positive values in the no_guests column.
- Duplication Check:
  - Verified that no duplicate rows existed in the dataset.
- Data Type Conversion:
  - Converted date columns from string format to datetime format for accurate analysis.
- Outlier Detection:
  - Replaced or corrected anomalies in revenue column using statistical techniques.
-Consistency Checks:
  - Verified consistency across datasets by checking unique IDs (e.g., hotel_id, room_id).

**3. Merging Datasets**
- Merged booking data with additional datasets (df_rooms, df_hotels, and df_date) to enhance the analysis scope.
- Dropped unnecessary columns (date and room_id) after merging.
 
**3. Exploratory Data Analysis**
- Occupancy Rates by Room Class:
  - Identified which room classes performed better in terms of occupancy.
- City-Wise Performance:
  - Evaluated city-level occupancy to identify underperforming and high-performing locations.
- Monthly Analysis:
  - Analyzed occupancy trends in specific months (e.g., July).
- Revenue Insights:
  - Analyzed revenue data by city, property_type etc.
  - Investigated weekday/weekend impacts on revenue
    
**4. Visualizations and Insights**
- Bar Charts:
  - Visualized distribution of booking by different platform.
  - Average hotel bookings during weekday and weekend in differnt cities.
- Time-Series Plots:
  - Analyzed revenue trends over months.
- Pie Chart:
  - Revenue distribution by booking platform
- Heatmaps:
  - Used heatmaps to show average revenue per property and room class.
  - Used heatmaps to show occupancy distribution across cities and room classes.



