# Customer Coupon Analysis

## Overview
This project aims to analyze customer coupon acceptance behavior based on various factors such as age, education level, and frequency of visits to bars, coffee houses, and restaurants. The analysis is performed using a Jupyter notebook.

## Dataset Description
The dataset contains the following columns:

- `destination`: The destination of the customer.
- `passanger`: The type of passenger (e.g., alone, with friends).
- `weather`: The weather condition.
- `temperature`: The temperature at the time of the trip.
- `time`: The time of the trip.
- `coupon`: The type of coupon offered.
- `expiration`: The expiration time of the coupon.
- `gender`: The gender of the customer.
- `age`: The age of the customer.
- `maritalStatus`: The marital status of the customer.
- `has_children`: Whether the customer has children.
- `education`: The education level of the customer.
- `occupation`: The occupation of the customer.
- `income`: The income level of the customer.
- `car`: The type of car the customer drives.
- `Bar`: Frequency of visits to bars (e.g., never, less1, 1~3, gt8).
- `CoffeeHouse`: Frequency of visits to coffee houses (e.g., never, less1, 1~3, gt8).
- `CarryAway`: Frequency of getting take-away food (e.g., never, less1, 1~3, gt8).
- `RestaurantLessThan20`: Frequency of visits to restaurants with an average bill less than $20.
- `Restaurant20To50`: Frequency of visits to restaurants with an average bill between $20 and $50.
- `toCoupon_GEQ5min`: Whether the time to reach the coupon location is greater than or equal to 5 minutes.
- `toCoupon_GEQ15min`: Whether the time to reach the coupon location is greater than or equal to 15 minutes.
- `toCoupon_GEQ25min`: Whether the time to reach the coupon location is greater than or equal to 25 minutes.
- `direction_same`: Whether the direction to the coupon location is the same as the destination.
- `direction_opp`: Whether the direction to the coupon location is opposite to the destination.
- `Y`: Whether the coupon was accepted (1 for accepted, 0 for not accepted).

## Analysis Steps
The analysis involves the following steps:

1. **Data Loading**: Load the dataset into a pandas DataFrame.
2. **Data Cleaning**: Handle missing or problematic data.
3. **Data Transformation**: Convert data types and filter data based on specific criteria.
4. **Exploratory Data Analysis (EDA)**: Analyze the data to understand customer behavior.
5. **Visualization**: Create visualizations to represent the data and findings.

## Example Analysis
Based on the data, the following observations were made:

1. **Acceptance Rate by Bar Frequency**:
   - The acceptance rate for people who visit bars 4-8 times and more than 8 times (`gt8`) is higher than for those who visit bars 1-3 times (`1~3`).

2. **Acceptance Rate for Bar Goers vs Non-Bar Goers**:
   - People who go to the bar have a higher acceptance rate than people who do not go to the bar.

3. **Acceptance Rate for Bar Goers with and without Kids**:
   - People who go to the bar with kids have a lower acceptance rate than people who go to the bar without kids.

4. **Acceptance Rate by Occupation**:
   - People who go to the bar with an occupation other than 'Farming Fishing & Forestry' have a higher acceptance rate than those with this occupation.

5. **Acceptance Rate by Age**:
   - People who go to the bar more than once a month and are above age 30 have a higher acceptance rate than people who go to the bar more than once a month and are below age 30.

## How to Run the Jupyter Notebook
1. **Install Dependencies**: Ensure you have the required libraries installed. You can install them using:
   ```bash
   pip install pandas matplotlib seaborn
   
2. Run Jupyter Notebook: Start the Jupyter Notebook server and open the prompt.ipynb file.

3. Execute Cells: Run the cells in the notebook to perform the analysis.

Conclusion
This project provides insights into customer coupon acceptance behavior based on various factors. The findings can help businesses tailor their marketing strategies to improve coupon acceptance rates.

License
This project is licensed under the MIT License.
