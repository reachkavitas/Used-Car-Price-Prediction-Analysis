# Used-Car-Price-Prediction-Analysis Report

# Introduction
The goal of this analysis was to identify the key factors influencing used car prices and to build a predictive model that can help dealers better understand and fine-tune their inventory. By leveraging various machine learning techniques and data preprocessing methods, I aimed to develop a robust model that could provide accurate price predictions and insights into what drives car values.

# Data Overview
The dataset used for this analysis includes various attributes of used cars, such as the year of manufacture, odometer reading, condition, fuel type, and vehicle type. The primary variable of interest is the car price, which I sought to predict based on these features.

# Key Findings
Primary Influencers of Car Price:

1.Year of Manufacture: Newer cars generally command higher prices. This relationship was captured moderately well by the model, indicating that age is a significant but not sole determinant of price.
2.Odometer Reading: As expected, higher mileage tends to lower a car’s value. The model consistently showed a negative correlation between odometer readings and car prices.
3.Condition: The condition of the vehicle plays a crucial role in determining its price. Cars in "new" or "excellent" condition are priced significantly higher than those in "fair" or "salvage" condition.
4.Fuel Type and Vehicle Type: Different fuel types and vehicle types also affect pricing. For instance, SUVs and trucks often have higher prices compared to sedans, and hybrid or electric vehicles might command a premium.

Model Performance:
After applying polynomial feature transformations and time series cross-validation, the model achieved a Test R-squared of 0.5952 and a Mean Absolute Error (MAE) of $5,778.51. This indicates that the model explains approximately 59.5% of the variance in car prices and makes predictions with an average error of around $5,779.
The model’s performance was relatively strong, especially after accounting for non-linear relationships between features and price using polynomial features.

Challenges Identified:
Inconsistent Performance Over Time: The model’s performance varied significantly across different time periods, with some folds in the time series cross-validation yielding negative R-squared values. This suggests that the market conditions or data characteristics changed during certain periods, affecting the model’s ability to predict accurately.
Potential Data Anomalies: The large discrepancies in cross-validation results may point to the presence of outliers or structural breaks in the data that need to be further investigated.

# Recommendations
Inventory Optimization:
1.Focus on Newer, Low-Mileage Cars: Since newer cars with lower mileage consistently fetch higher prices, prioritize acquiring vehicles that fit this profile.
2.Condition Matters: Emphasize sourcing cars in "excellent" or "new" condition, as these are significantly more valuable.
3.Diversify Fuel and Vehicle Types: Consider maintaining a diverse inventory with a mix of fuel types and vehicle types, especially as demand for SUVs, trucks, and hybrid/electric vehicles continues to grow.

Further Model Refinement:
Address Inconsistencies: Investigate the time periods where the model performed poorly to identify any underlying causes, such as market shifts or data quality issues.
Advanced Modeling: Explore more advanced time series models or ensemble methods that may provide more stable performance across different market conditions.

Continuous Monitoring:
Regularly update the model with new data to capture any emerging trends in the used car market. Continuous retraining will help maintain the model's accuracy over time.

# Conclusion
The analysis provides valuable insights into the factors that drive used car prices, offering a foundation for dealers to optimize their inventory. While the predictive model performed reasonably well, there is room for further improvement, particularly in addressing the variability observed across different time periods. By applying these findings and recommendations, dealers can better align their inventory with market demands and maximize profitability.
