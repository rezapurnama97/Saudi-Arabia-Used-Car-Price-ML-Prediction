# Saudi Arabia Used Car Price Prediction
predicting the selling price of used cars on the https://syarah.com/ website
![Gambar Syarah](https://i0.wp.com/www.menabytes.com/wp-content/uploads/2018/05/Syarah-Series-A.jpg?fit=1000%2C500&ssl=1&resize=1280%2C720)

# Context 
---

Based on article titled  [Saudi Arabia's Used Cars Sales Market is Poised to Take Off](https://www.consultancy-me.com/news/5464/saudi-arabias-used-cars-sales-market-is-poised-to-take-off), due to financial constraints and the current pandemic scenario, many buyers are postponing the purchase of new cars and are looking to buy high-quality used cars at a reasonable price. The used car market is likely to expand in the next five years as online players provide good value for money. Saudis generally replace their cars every 2-4 years, while expatriates change their cars after 4 years on average. However, this trend is likely to change as younger Saudis enter the workforce and women are allowed to drive. The average age of most second-hand sales is likely to move towards 5-6 years. 


Syarah, being an online marketplace for selling cars in Saudi Arabia, plays a crucial role in the expanding used car market. With the growing trend of buyers opting for high-quality used cars and the changing dynamics of car ownership in the country, Syarah's platform serves as a convenient and efficient solution for sellers and buyers. However, to ensure the success of the platform, it is important for sellers to accurately determine the pricing of their cars. This will not only attract potential buyers but also maintain Syarah's performance by sustaining visitor and buyer numbers, ultimately leading to increased profitability for the company.

# Problem
---

 Determining the right selling price for a car based on its specifications is challenging for sellers on the Syarah platform. Sellers may struggle to set competitive prices, leading to potential lack of interest from buyers if the price is too high or disproportionate profit if the price is too low. This can result in decreased transactions and negatively impact Syarah's revenue. __How does Syarah.com determine the right car selling price based on existing specifications from previous sales data?__

# Goals
---
Based on the problem, **Syarah.com needs to introduce an innovative tool that can accurately predict car prices**. This tool will provide guidance to sellers in determining competitive selling prices that reflect the true value of their cars. Additionally, it will assist buyers in making informed decisions by ensuring they obtain fair purchase prices aligned with market value. By achieving these goals, Syarah.com aims to create transparency and fairness in car transactions for both sellers and buyers, while generating sustainable profits for Syarah.com as an online marketplace platform for cars.

# Conclusion

- The best model to be implemented to this dataset is Catagory Boost Regressor with the default parameter.

- According to feature importance to Price, "Year" feature has a significant impact on the price of used car sales.

- A dataset with a column of prices containing zero values cannot be used for machine learning because we only want to predict data with real numbers. However, this has the effect of making the dataset very small (only 3757 rows of data).

- This machine learning modeling is using MAPE (Mean Absolute Percentage Error) as matrix scoring because we want to understand the percentage error of predictions relative to the actual values. If it is important to measure the relative percentage error in predicting used car prices, especially in the context of comparison or performance analysis, then MAPE can be used. For example, if a company wants to assess the accuracy of a used car price prediction model for different car brands engine size or Mileage, MAPE would be a suitable metric. By calculating the percentage error, the company can compare the model's performance across different segments and identify any variations in prediction accuracy.

- The results show that after tuning the hyperparameters of the model, the MAPE slight increased from 17.76% to 18.14%, indicates that the accuracy of the model has dropped 
0.58%. This suggests that the hyperparameter tuning process was failed in improving the model's performance, and updated model can't make better predictions on new data.Therefore we will suggest using the model before tuning as a machine learning model for predicting second hand car prices.

-  Since the results of the machine learning modeling using the CatBoost algorithm, with the MAPE evaluation score before tuning showing a value below 20%, specifically 17.76%, this modeling is considered as good forecasting and is suitable for implementation on the Syara.com website.
