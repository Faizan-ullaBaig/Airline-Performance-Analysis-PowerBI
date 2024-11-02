# Airline Performance Analysis using Power BI
An in-depth Power BI project to analyze and optimize airline performance, with insights into flight operations, passenger management, and booking trends.

## Introduction
This project provides a comprehensive analysis of key aspects of airline operations—ranging from flight scheduling and ticket bookings to passenger management. Using Power BI's powerful data transformation, visualization, and analytical capabilities, I created an interactive dashboard designed to uncover operational bottlenecks, reveal booking trends, and generate data-driven insights essential for enhancing airline performance and boosting customer satisfaction.

## Problem Statement
In a highly competitive and dynamic industry, efficient management of airline operations is critical to maintaining customer satisfaction and enabling strategic, data-driven decision-making. Daily operations include flight scheduling, ticketing, and passenger management, and without a streamlined way to analyze these metrics, it's challenging to make timely improvements. By leveraging Power BI for this analysis, I aim to deliver actionable insights that allow stakeholders to monitor airline performance effectively, optimize resources, and make informed decisions.

## Objective
The main objectives of this project are:
1. **Analyze airline operations data**, focusing on flight performance metrics, passenger data, and ticketing trends.
2. **Create a Power BI dashboard** that offers real-time insights and enables interactive data exploration.
3. **Provide actionable insights** to guide decisions on improving flight punctuality, enhancing customer experience, and optimizing ticketing processes.

## Datasets
The project utilizes three primary datasets:
1. **Flight Information**: Contains details on individual flights, including `FlightID`, `FlightNumber`, `Airline`, `Destination`, and `Status`.
2. **Passenger Information**: Provides passenger details, such as `PassengerID`, `FlightID`, and `SeatNumber`, allowing a passenger-to-flight mapping.
3. **Ticket Information**: Includes booking information with fields like `TicketID`, `FlightID`, and `BookingStatus`, facilitating tracking of booking trends.

## Project Workflow and Key Tasks
### 1. Data Extraction and Transformation
   - **Loading Data**: Imported datasets into Power BI from CSV files.
   - **Data Cleaning**: Removed duplicate entries, handled missing values, and formatted columns consistently.
   
### 2. Creating Conditional and Custom Columns
   - **Conditional Columns**: Classified flights as “Best” or “To be Improved” based on their on-time performance. This allowed quick filtering and analysis of punctual flights.
   - **Custom Columns from Examples**: Created a custom column to extract the flight number substring, ensuring data consistency.

### 3. Merging Queries and Columns
   - **Query Merging**: Merged the `Flight Information` and `Passenger Information` tables on `FlightID` to form a unified dataset for further analysis.
   - **Column Merging**: Combined `SeatNumber` and `PassengerID` columns to create unique identifiers for each passenger, simplifying passenger-specific analysis.

### 4. DAX Calculations for Insights
   - **Total Passengers per Flight**: Calculated the total number of passengers for specific flights using DAX, for example, analyzing flights like `FL1276`.
   - **Total Tickets Booked**: Aggregated total tickets booked across all flights.
   - **Filtered Table for Best Flights**: Created a filtered table that shows only the best flights, based on on-time performance.

### 5. Visualizations
   - **Multi-Card Visual**: Showed metrics such as passenger count and flight numbers for each airline, allowing for a quick overview of airline activity.
   - **Bar Chart**: Compared passenger counts across airlines to identify the busiest airlines.
   - **Donut Chart**: Displayed the distribution of ticket booking statuses, providing insight into booking trends and completion rates.

### 6. Advanced Visualizations: Decomposition Tree and Key Influencer
   - **Decomposition Tree**: Analyzed the number of flights by breaking them down by airline and destination. This highlighted key patterns in flight distribution.
   - **Q&A Feature**: Used the Q&A visual to answer natural language queries about booking statuses, adding an interactive component to the dashboard.

### 7. Interactive Features: Slicers, Bookmarks, and Drill Through
   - **Slicers**: Implemented a slicer for filtering data by destination, total passengers, and total flights for selected airlines.
   - **Bookmarks**: Created bookmarks to save different views of the report, allowing for fast and user-friendly navigation.
   - **Drill-Through**: Enabled drill-through functionality to navigate from a high-level view of all airlines to detailed views of specific airlines, destinations, and flight counts.

### 8. Final Report and Dashboard
   - **Workspace Creation**: Established a new workspace named “Airline” in Power BI Service, organizing all reports and datasets in a dedicated space.
   - **Dashboard Design**: Integrated key visuals, Q&A, and a summary of insights, making it easy for users to access relevant data at a glance.
   - **Role-Level Security (RLS)**: Configured RLS to limit access to Airline A’s data for specific users, ensuring secure data viewing.
   - **Scheduled Refresh**: Set up a daily refresh at 5 PM to keep data up-to-date, guaranteeing that the analysis reflects the latest information.

## Key Findings and Insights
1. **On-Time Performance**: Identified airlines with strong on-time performance, allowing management to recognize efficiency and reward reliability.
2. **Passenger Distribution**: Visualized passenger volume across airlines, highlighting where resources might need to be increased to support high traffic.
3. **Booking Trends**: Analyzed booking statuses, identifying patterns that can help reduce cancellations and delays through improved processes.
4. **Popular Destinations**: Showed the most frequently traveled routes, providing insights for route optimization and capacity planning.

## Visuals
Here are some key visuals from the project:
   
   ![Ticket Booked](Ticket%20booked.png)
   
   ![Slicer](Slicer.png)
   
   ![Dashboard Overview](Image1.png)
   
   ![Decomposition Tree](Decomposition%20Tree.png)
   
   ![Count of Booking Status](Count%20of%20booking%20status.png)

## Conclusion
This project provided valuable insights into airline operations, passenger distribution, and booking trends. By creating a Power BI dashboard with real-time, interactive visualizations, stakeholders can now monitor performance and make data-driven decisions to improve customer satisfaction and operational efficiency. This analysis is a foundation for more granular, predictive insights into future airline performance.
