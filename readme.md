# Uber City Supply and Demand Data Analysis

This project analyzes city supply and demand data provided by Uber to answer several key questions related to trip patterns, driver behavior, and optimal scheduling. The analysis is based on a dataset covering a two-week period.

## Dataset

The analysis uses the `dataset_1.csv` file, which contains hourly data with the following columns:

- **Date**: The date of the observation.
- **Time (Local)**: The local time (start of the hour).
- **Eyeballs**: Number of people who opened the Uber app.
- **Zeroes**: Number of people who did not see any available cars.
- **Completed Trips**: Number of completed trips.
- **Requests**: Number of trip requests.
- **Unique Drivers**: Number of unique drivers logged in.

## Analysis Questions and Answers

The project addresses the following questions:

1.  **Which date had the most completed trips during the two week period?**
    *   Answer: 22 September 2012

2.  **What was the highest number of completed trips within a 24 hour period?**
    *   Answer: 278 Completed Trips between Sep 21, 2012 5 PM - Sep 22, 2012 5 PM

3.  **Which hour of the day had the most requests during the two week period?**
    *   Answer: Hour 23, with 184 requests

4.  **What percentages of all zeroes during the two week period occurred on weekend (Friday at 5 pm to Sunday at 3 am)?**
    *   Answer: 44.86 %

5.  **What is the weighted average ratio of completed trips per driver during the two week period?**
    *   Answer: Weighted Average Ratio is 0.83

6.  **In drafting a driver schedule in terms of 8 hours shifts, when are the busiest 8 consecutive hours over the two week period in terms of unique requests?**
    *   Answer: Busiest 8 consecutive hours with 207 unique requests each are:
        1.  September 21, 2012 5 PM - September 22, 2012 1 AM
        2.  September 22, 2012 7 PM - September 23, 2012 3 AM

7.  **True or False: Driver supply always increases when demand increases during the two week period.**
    *   Answer: FALSE. Generally, driver supply increases when demand increases but NOT always.

8.  **In which 72 hour period is the ratio of Zeroes to Eyeballs the highest?**
    *   Answer: Highest Zeroes to Eyeballs ratio is: September 15, 2012 5 AM - September 18, 2012 5 AM

9.  **If you could add 5 drivers to any single hour of every day during the two week period, which hour should you add them to?**
    *   Answer: Since, Hour 23 has the lowest driver availability to people looking for rides (Eyeballs), adding 5 more drivers to hour 23 would make most sense to improve that ratio.

10. **True or False: There is exactly two weeks of data in this analysis.**
    *   Answer: TRUE, exactly 14 days between Sep 10, 2012 7 AM - Sep 24, 2012 7 AM.

11. **Looking at the data from all two weeks, which time might make the most sense to consider a true "end day" instead of midnight?**
    *   Answer: From the graphs and rank analysis, we see the supply and demand is at minimum in early hours of morning, between 4 AM - 5 AM. Hence, instead of midnight, this should be the "true end" day.

## Libraries Used

-   numpy
-   pandas
-   datetime
-   matplotlib

## Code Structure

The notebook is organized into sections for:

-   Loading necessary libraries.
-   Loading and inspecting the dataset.
-   Data preprocessing (handling missing values and duplicates).
-   Addressing each analysis question with code and a written answer.