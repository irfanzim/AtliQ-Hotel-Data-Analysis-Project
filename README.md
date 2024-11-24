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
![image](https://github.com/user-attachments/assets/3dbf8856-75f1-45e0-979d-9f02177b21a0)

- Handling Inconsistencies:
  - Removed rows where successful_bookings exceeded capacity.
  - Converted negative values to positive values in the no_guests column.
![image](https://github.com/user-attachments/assets/2f4353f3-2f54-47f2-b1b2-6f809add0333)

- Duplication Check:
  - Verified that no duplicate rows existed in the dataset.
![image](https://github.com/user-attachments/assets/76d1bf72-7f7a-44e4-a5a0-ab6922169a1e)

- Data Type Conversion:
  - Converted date columns from string format to datetime format for accurate analysis.
 ![image](https://github.com/user-attachments/assets/2f37c229-7e16-4da5-9d1b-2874f7a00b6a)

- Outlier Detection:
  - Removed or corrected anomalies in revenue column using statistical techniques.
![image](https://github.com/user-attachments/assets/064fcf28-586b-41bd-8945-615fcc55691b)


- Consistency Checks:
  - Verified consistency across datasets by checking unique IDs (e.g., booking id).

**3. Merging Datasets**
- Merged booking data with additional datasets (df_rooms, df_hotels, and df_date) to enhance the analysis scope.
![image](https://github.com/user-attachments/assets/20c519ff-e2fd-4934-9658-99309393a71a)

- Dropped unnecessary columns (date and room_id) after merging.
 
**3. Exploratory Data Analysis**
- Occupancy Rates by Room Class:
  - Identified which room classes performed better in terms of occupancy.
![image](https://github.com/user-attachments/assets/d3cf967c-8ffe-4242-ae12-7460123716bf)

- City-Wise Performance:
  - Evaluated city-level occupancy to identify underperforming and high-performing locations.
![image](https://github.com/user-attachments/assets/08b06007-8fde-4804-93df-0631c810f9df)

- Monthly Analysis:
  - Analyzed occupancy trends in specific months (e.g., July).
- Revenue Insights:
  - Analyzed revenue data by city, property_type etc.
![image](https://github.com/user-attachments/assets/4eebedc5-1d4f-482c-bfd2-e5438313d677)

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












