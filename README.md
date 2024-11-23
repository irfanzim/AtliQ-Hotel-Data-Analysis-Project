# AtliQ-Hotel-Data-Analysis-Project (Python Project)

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
 ![image](https://github.com/user-attachments/assets/2f37c229-7e16-4da5-9d1b-2874f7a00b6a)

- Outlier Detection:
  - Replaced or corrected anomalies in revenue column using statistical techniques.
- Consistency Checks:
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
  
![image](https://github.com/user-attachments/assets/afe955f6-bf70-40a7-807e-e549b42a535a)

![image](https://github.com/user-attachments/assets/585f28cd-cbcb-4563-b3b6-702ee65ee32b)
- Time-Series Plots:
  - Analyzed revenue trends over months.

![image](https://github.com/user-attachments/assets/782212b6-718e-479e-9aa3-41e8443053c4)

- Pie Chart:
  - Revenue distribution by booking platform

 ![image](https://github.com/user-attachments/assets/22e7de17-f466-4cc4-b801-a427ba9a9a0d)
 
- Heatmaps:
  - Used heatmaps to show average revenue per property and room class.
  - Used heatmaps to show occupancy distribution across cities and room classes.
 
![image](https://github.com/user-attachments/assets/7463286a-8ba7-4648-8fc9-d9d5bf26302d)

![image](https://github.com/user-attachments/assets/a1c398dc-2317-47fe-b609-6cd551ee4f55)

## **Key Insights**
- Highest occupancy rates observed in Presidential suites (59.28%), followed by Premium rooms (58.03%).
- Delhi had the highest occupancy rate (61.51%), while Bangalore lagged behind (56.33%).
- Weekend occupancy was significantly higher (73.96%) compared to weekdays (51.81%).
- Revenue decreased in Jun 22, followed by an upward trend in July 22
- Atliq Exotica contributed the highest revenue at 320,279,488, while Atliq Seasons contributed the least at 66,125,495.
- MakeMyTrip generates the second-largest share of revenue, accounting for 19.9%.
- Atliq Exotica consistently generated the highest average revenue across all room categories, with the Presidential room category being the most lucrative.

## **Key Recommendations**
- Offer dynamic pricing based on demand patterns observed in weekends.
- Leverage loyalty programs tailored for weekend travelers, who form a significant portion of bookings.
- Invest in promotional offers and loyalty programs for underperforming cities like Bangalore.
- Highlight Presidential suites during high-demand seasons to maximize revenue.

## **Summary of Skills Demonstrated:**
- **Data Cleaning:** Handling inconsistent and duplicate data.
- **Data Integration:** Merging multiple datasets into a cohesive structure.
- **EDA:** Aggregating, grouping, and analyzing data trends.
- **Feature Engineering:** Creating meaningful new columns (OCC%).
- **Statistical Analysis:** Calculating means, proportions, and rates.
- **Python Libraries:** Proficiency in pandas, and visualization libraries like matplotlib.
- **Business Analytics:** Applying data insights to real-world problems for strategic recommendations.












