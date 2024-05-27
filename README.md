# Supply Data Analysis - Ride-Hailing Service

This project analyzes supply and demand data for a ride-hailing service. The goal is to understand the dynamics of driver availability versus rider demand and identify opportunities for improvement.

## Data

The project uses two CSV files:

* **Hourly_DriverActivity_1.csv**: Contains hourly data on driver activity, including active drivers, online hours, booked hours, waiting hours, busy hours, rides per online hour, and finished rides.
* **Hourly_OverviewSearch_1.csv**: Contains hourly data on rider search activity, including the number of users who saw 0 cars, the number of users who saw +1 cars, and the coverage ratio.

## Objectives

* **Identify Undersupplied Hours:** Determine the 36 hours in a week with the highest undersupply based on driver activity.
* **Visualize Supply and Demand:**  Create a 24-hour curve illustrating the average supply (drivers) and demand (riders) to highlight mismatches.
* **Analyze Peak Hours:** Identify the peak hours with the highest demand and estimate the number of additional driver hours needed to achieve a high coverage ratio during those times.
* **Calculate Guaranteed Earnings:** Estimate the guaranteed hourly earnings that can be offered to drivers during the 36 hours with the highest demand without losing money.
* **Extra Hours for Capturing Demand:** Calculate the number of extra driver hours needed to capture missed demand during peak hours.

## Analysis

The analysis involves:

1. **Data Cleaning:** Handling missing values and renaming columns for clarity.
2. **Exploratory Data Analysis (EDA):**  
    * Plotting the most undersupplied hours.
    * Creating 24-hour curves for average supply and demand.
    * Plotting the relationship between supply ratio and online hours.
    * Analyzing peak hours and calculating additional driver hours needed for high coverage.
    * Estimating guaranteed hourly earnings for drivers during peak hours.
    * Plotting the hours needed to capture missed demand.

## Results

The analysis will reveal key insights:

* **Undersupply:** Specific hours of the week where demand exceeds supply.
* **Peak Demand:**  Hours with the highest demand and potential for missed rides.
* **Earnings Potential:** Hourly earnings drivers could receive during peak hours without impacting platform profitability.
* **Extra Hours Needed:**  The required increase in driver hours to meet demand during peak times.

## Recommendations

Based on the analysis, recommendations will be made for:

* **Driver Incentives:** Strategies to motivate drivers to work during undersupplied hours.
* **Demand Management:**  Adjustments to rider pricing or promotions to manage demand during peak periods.

## Algorithms for Demand and Supply Optimization

Several algorithms can be employed to optimize demand and supply in ride-hailing services:

**1. Surge Pricing:**

* **Concept:**  Dynamically increase fares during peak demand hours to incentivize more drivers to come online.
* **How it works:** The platform analyzes real-time data (driver availability, rider requests) and adjusts fares accordingly.
* **Benefits:** 
    * Balances supply and demand by attracting more drivers.
    * Generates higher revenue for the platform and drivers.
* **Challenges:** 
    * Requires careful calibration to avoid pricing riders out of the market.
    * May lead to customer dissatisfaction if perceived as unfair.

**2. Driver Incentive Programs:**

* **Concept:** Offer bonuses, guaranteed earnings, or other incentives to attract drivers to specific time slots or areas.
* **How it works:**  The platform can offer:
    * **Guaranteed earnings:** A minimum amount paid to drivers for working during specific hours.
    * **Peak bonuses:**  Additional payments for rides completed during high-demand periods.
    * **Referral bonuses:** Rewards for drivers who refer new drivers to the platform.
* **Benefits:** 
    * Improves driver retention.
    * Encourages drivers to work during high-demand periods.
* **Challenges:**
    * Can be costly for the platform.
    * Requires monitoring to ensure effectiveness.

**3. Rider Incentives:**

* **Concept:** Offer promotions or discounts to riders during off-peak hours to stimulate demand.
* **How it works:**
    * **Early bird discounts:**  Reduced fares for rides booked before a certain time.
    * **Late night specials:**  Discounted rides during late-night hours.
    * **Promotional codes:**  Codes offering discounts to specific rider groups.
* **Benefits:** 
    * Smooths out demand and creates a more consistent workload for drivers.
    * Attracts new customers.
* **Challenges:**
    * Can decrease revenue for the platform if not managed carefully.
    * Requires targeted campaigns to be effective.

**4. Predictive Models:**

* **Concept:**  Use historical data and machine learning to forecast demand and driver availability.
* **How it works:** The platform builds models to predict:
    *  Peak demand times and locations.
    *  Driver availability patterns.
* **Benefits:**
    * Allows for proactive driver recruitment.
    * Enables targeted promotions and incentives.
* **Challenges:**
    * Requires expertise in data science and machine learning.
    * Models need to be updated regularly.

**5. Geographic Routing:**

* **Concept:**  Optimize driver routes to ensure they are positioned in high-demand areas.
* **How it works:**  The platform uses algorithms to:
    *  Calculate the optimal routes based on rider demand and driver location.
    *  Direct drivers to areas where they are most likely to find riders.
* **Benefits:** 
    * Reduces wait times for riders.
    * Improves driver efficiency.
* **Challenges:**
    * Requires real-time data and advanced routing algorithms.

## Next Steps

* **More Data:** Incorporate data from multiple weeks or regions to enhance the analysis.
* **Driver Preferences:** Explore factors influencing driver availability, such as preferred time slots or geographic areas.
* **Dynamic Pricing:**  Implement dynamic pricing strategies that adjust fares based on real-time supply and demand.

## Project Structure

The project includes the following files:

* **Supply-demand.py**:  The main jupyter Notebook containing the analysis code.
* **README.md**: This file.
* **Hourly_DriverActivity_1.csv**: Data on driver activity.
* **Hourly_OverviewSearch_1.csv**: Data on rider search activity.

## Getting Started

1. Install the required libraries:
   ```bash
   pip install pandas matplotlib seaborn
   ```
2. Run the analysis script:
    ```bash
   python Supply-demand.py
   ```
3. Examine the generated plots and results
    **Remember:** Replace the placeholder file names `Hourly_DriverActivity_1.csv` and `Hourly_OverviewSearch_1.csv` with the actual names of your data files.