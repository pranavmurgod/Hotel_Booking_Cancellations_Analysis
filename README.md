# Hotel_Booking_Cancellations_Analysis

This project is a data analysis and visualization initiative focused on understanding hotel booking trends, specifically investigating factors associated with reservation cancellations. Using Python libraries like Pandas, Matplotlib, and Seaborn, I conducted a complete data cleaning, exploratory data analysis (EDA), and developed visualizations to reveal patterns in customer behavior and booking details.

## Project Overview

This analysis is based on a hotel booking dataset that contains information about 81,571 reservations, including various features related to booking status, customer demographics, booking channels, and reservation details. The aim of this project is to identify key insights into reservation cancellations and provide actionable findings for hotel management and marketing strategies.

## Tools & Libraries Used

- **Pandas**: For data loading, manipulation, and cleaning.
- **Matplotlib**: For plotting and visualizing data insights.
- **Seaborn**: For creating more advanced and styled visualizations.
- **PyCharm & DataSpell**: IDEs used for developing the project. Jupyter Notebook was integrated into the PyCharm Community Edition in a read-only mode, and fully supported in DataSpell.

## Key Project Phases

### 1. **Data Import & Initial Exploration**
   - Loaded the hotel booking data from a CSV file using Pandas.
   - Reviewed initial data using `df.head()`, `df.tail()`, `df.info()`, and `df.describe()` to understand the data structure, column types, and check for null values.

### 2. **Data Cleaning**
   - Removed unnecessary columns (`company` and `agent`) and dealt with missing values by dropping incomplete rows.
   - Converted the `reservation_status_date` column to a `datetime` format for time-series analysis.
   - Filtered extreme outliers in the `adr` (Average Daily Rate) column to ensure accurate analysis.

### 3. **Exploratory Data Analysis (EDA)**
   - **Data Distribution**: Inspected unique values for categorical variables such as `hotel`, `meal`, `market_segment`, `country`, and `reservation_status`.
   - **Null Value Analysis**: Calculated and addressed null values across columns, ensuring clean data for analysis.
   - **Cancellation Rate**: Calculated the percentage of bookings canceled and visualized the counts for canceled vs. not canceled bookings.

### 4. **Data Analysis and Visualization**

   #### Key Analyses:
   - **Reservation Status Analysis**: Created a bar chart to visualize counts of canceled vs. not canceled reservations, with approximately 53.3% cancellation rate.
   - **Hotel Type Comparison**: Analyzed the cancellation patterns for `City Hotel` vs. `Resort Hotel`, showing that city hotels had higher cancellation rates.
   - **Average Daily Rate (ADR) Trends**: Plotted ADR trends over time, segmented by hotel type. This helped reveal seasonal trends and rate differences between `City Hotel` and `Resort Hotel`.
   - **Monthly Reservation Patterns**: Visualized reservation cancellations on a monthly basis, identifying peak months for cancellations and drawing insights into seasonal booking behaviors.
   - **Top 10 Countries with Most Cancellations**: Created a pie chart to show the top countries contributing to cancellations, providing geographic insights for targeted marketing.

### 5. **Detailed Visualizations**
   - **Reservation Status by Hotel Type**: Used `sns.countplot` to create visual comparisons of cancellations between `Resort Hotel` and `City Hotel`.
   - **ADR by Cancellation Status**: Explored the ADR trends for canceled and not-canceled bookings, with a focus on identifying periods with high ADRs and high cancellation rates.
   - **Monthly ADR Trends for Cancellations**: Visualized monthly ADR variations for canceled reservations, helping identify when the highest revenue was lost due to cancellations.
   - **Market Segment Analysis**: Examined the distribution of `market_segment` for canceled bookings, gaining insights into segments with the highest cancellation risks.

## Results & Insights

- **High Cancellation Rate**: Around 53% of bookings were canceled, with city hotels exhibiting a higher cancellation rate than resort hotels.
- **Seasonal Trends**: Peak months with high cancellation rates were identified, suggesting potential overbooking strategies during high-demand seasons.
- **Geographic Trends**: Certain countries showed higher cancellation rates, highlighting the need for geographically targeted promotions or flexible policies.
- **Market Segment Impact**: The `Online TA` segment exhibited a high cancellation rate, suggesting the potential for revisiting agreements with online travel agencies or offering special incentives to reduce cancellations.

## Conclusion

This project provided actionable insights into hotel booking cancellations by using data cleaning, transformation, and visualization techniques. Key findings suggest that hotels may benefit from targeted policies for certain months, flexible booking options for customers from high-cancellation countries, and strategic planning to accommodate high-demand periods effectively.

## Future Work

- **Predictive Analysis**: Integrate machine learning models to predict cancellation probability based on booking attributes.
- **Advanced Segmentation**: Further analyze cancellations by combining additional features, like `customer_type` and `previous_cancellations`.
- **Reservation Status Prediction**: Develop a model to recommend actions for hotels to lower cancellation rates.

