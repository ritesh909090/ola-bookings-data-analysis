# Ola Bookings Data Analysis

## Project Overview
This project analyzes Ola ride-booking data for **July 2024** using SQL and Power BI. The goal is to explore booking activity, ride outcomes, vehicle performance, revenue/payment patterns, cancellation behaviour, and ratings through SQL analysis and an interactive dashboard.

> **Dataset note:** The dataset is a synthetic/tutorial dataset and should not be interpreted as official Ola operational data.

## Tools Used
- **SQL / MySQL** — querying the data, aggregation, filtering, grouping, and creating views for analysis.
- **Microsoft Power BI** — building the interactive dashboard and report pages.
- **DAX** — creating KPI measures used in Power BI visuals/cards.

## Dataset
The project dataset includes booking-level fields such as:
- Date and time
- Booking ID and booking status
- Customer ID
- Vehicle type
- Pickup and drop locations
- V_TAT and C_TAT
- Customer and driver cancellation fields
- Incomplete ride flag and reason
- Booking value and payment method
- Ride distance
- Driver and customer ratings

The dashboard date filter is set to **July 1–31, 2024**.

## SQL Analysis
The project includes SQL analysis for these business questions:

1. Retrieve all successful bookings.
2. Calculate average ride distance by vehicle type.
3. Count rides cancelled by customers.
4. Identify the top 5 customers by number of bookings.
5. Count driver cancellations due to personal and car-related issues.
6. Find maximum and minimum driver ratings for Prime Sedan bookings.
7. Retrieve rides paid using UPI.
8. Calculate average customer rating by vehicle type.
9. Calculate total booking value from successful rides.
10. List incomplete rides with their reasons.

SQL views were created to save and reuse the results of the analysis.

## Power BI Dashboard
The dashboard is organized into five report pages:

### 1. Overall
- Total bookings
- Total booking value
- Booking status breakdown
- Ride volume over time

### 2. Vehicle Type
- Total booking value by vehicle type
- Successful booking value by vehicle type
- Average ride distance
- Total distance travelled

### 3. Revenue
- Booking value by payment method
- Top 5 customers by booking value
- Daily ride-distance trend

### 4. Cancellation
- Customer cancellation reasons
- Driver cancellation reasons
- Total bookings, successful bookings, cancelled bookings, and cancellation rate KPI cards

### 5. Ratings
- Driver ratings by vehicle type
- Customer ratings by vehicle type

DAX was used to create dashboard KPIs. The report includes date slicers for interactive filtering.

## Dashboard Screenshots

### Overall
![Overall Dashboard](screenshots/overall.png)

### Vehicle Type
![Vehicle Type Dashboard](screenshots/vehicle_type.png)

### Revenue
![Revenue Dashboard](screenshots/revenue.png)

### Cancellation
![Cancellation Dashboard](screenshots/cancellation.png)

### Ratings
![Ratings Dashboard](screenshots/ratings.png)

## Selected Dashboard Observations
Based on the displayed dashboard values:
- Total bookings: **103,024**
- Successful bookings: **63,967**
- Cancelled bookings (KPI): **28,933**
- Cancellation rate (KPI): **28.08%**
- Total booking value displayed: approximately **₹35M**
- The booking-status chart shows successful bookings at approximately **62.09%**.
- The ratings page shows vehicle-type ratings clustered around **4.0** for both customers and drivers.

These are observations from the dashboard screenshots and are not independently validated against the raw dataset.

## Project Workflow
1. Review the dataset fields and business questions.
2. Use SQL to query and aggregate booking-level data.
3. Create reusable SQL views for selected analysis outputs.
4. Build KPI measures in DAX.
5. Create and organize the Power BI visuals into five report pages.
6. Add date filtering and page navigation for interactive exploration.

## Skills Demonstrated
- SQL querying and aggregation
- Data analysis and business-question framing
- KPI creation with DAX
- Power BI dashboard development
- Data storytelling and visual organization
- Interactive reporting with slicers

## Limitations
- The data is synthetic/tutorial data, not official Ola data.
- Dashboard figures and observations should be validated against the raw dataset before being used as formal business conclusions.
- The dashboard screenshot displays a July 2024 date range.

## How to Use
1. Open the Power BI `.pbix` file.
2. Use the date slicer to select a date range.
3. Navigate between Overall, Vehicle Type, Revenue, Cancellation, and Ratings pages.
4. Explore the KPIs and visuals to investigate ride-booking patterns.

## Author
**Data Analytics Portfolio Project**  
Tools: SQL (MySQL), Power BI, DAX

