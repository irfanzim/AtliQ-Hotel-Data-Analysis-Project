# AtliQ-Hotel-Data-Analysis-Project

## **Project Overview:**

- **Client:** Atliq Grands, a major Indian hotel chain.
- **Objective:** Analyze hotel booking data to uncover key insights that can drive customer retention and increase revenue.

## **Problem Statement**

- Atliq Grands is facing stiff competition and declining revenue.
- The company seeks a data-driven approach to identify key factors impacting performance and make strategic improvements.

## **Datasets Overview**
The project uses a combination of dimensional and fact tables:

- **dim_date.csv:** Date information with fields such as date, month, week and date type (weekday/weekend).
- **dim_hotels.csv:** List of hotels with their respective IDs, names, category and city.
- **dim_rooms.csv:** Room details including room category and type.
- **fact_aggregated_bookings.csv:** Aggregated booking data with property id, total bookings, capacity etc.
- **fact_bookings.csv:** Detailed booking transactions with information on guests, room categories, booking dates, revenue etc.

## **Key Steps in the Project**
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
- Data Type Conversion:
  - Converted date columns from string format to datetime format for accurate analysis.
- Outlier Detection:
  - Detected negative values in the no_guests column.
  - Replaced or corrected these anomalies using statistical techniques.
-Consistency Checks:
  - Verified consistency across datasets by checking unique IDs (e.g., hotel_id, room_id).



