# Flight Revenue Analysis Report

![Flights Revenue Dashboard .png](Flight%20Revenue%20Analysis%20Report%2018c4799bb267808eb79ae64d3557d1ed/Flights_Revenue_Dashboard_.png)

# Data Extraction and Transformation

The dataset for this analysis was extracted from a SQL database using the following query:

![flight sql query.png](Flight%20Revenue%20Analysis%20Report%2018c4799bb267808eb79ae64d3557d1ed/flight_sql_query.png)

The query retrieves data from the `flight_revenue` table, groups it by `id`, and limits the output to 15 rows. The extracted data was then exported to a **CSV file**, which was later converted into an **Excel (.xlsx) file** for further analysis.

# Data Cleaning in Excel

To ensure consistency and readability in the dataset, the following data cleaning steps were performed in Excel:

1. **Standardizing Text Formatting:**
    - All text-based data (such as destination names) were formatted using the `UPPER()` and `PROPER()` functions to ensure uniform capitalization.

![data cleaning 1.png](Flight%20Revenue%20Analysis%20Report%2018c4799bb267808eb79ae64d3557d1ed/data_cleaning_1.png)

1. **Removing Underscores:**
    - Column names that contained underscores were cleaned using the `SUBSTITUTE()` function to replace underscores with spaces.

![data cleaning 2.png](Flight%20Revenue%20Analysis%20Report%2018c4799bb267808eb79ae64d3557d1ed/data_cleaning_2.png)

1. **Formatting for Presentation:**

- All text was standardized to the **Calibri** font for readability.
- The dataset was arranged into a presentable table format.

![data cleaning 3.png](Flight%20Revenue%20Analysis%20Report%2018c4799bb267808eb79ae64d3557d1ed/data_cleaning_3.png)

## **Calculating Key Performance Indicators (KPIs)**

After cleaning the data, the next step was to calculate the **Total Revenue** and identify key business insights.

### **1. Calculating Total Revenue**

To calculate the **total revenue per destination**, a new column was created using the **SUM function** to sum up revenue from different seating classes and cargo revenue.

![total revenue.png](Flight%20Revenue%20Analysis%20Report%2018c4799bb267808eb79ae64d3557d1ed/total_revenue.png)

![total revenue 2.png](Flight%20Revenue%20Analysis%20Report%2018c4799bb267808eb79ae64d3557d1ed/total_revenue_2.png)

- This formula was then dragged down across all rows to apply it to the entire dataset.

---

### **2. Identifying the Destination with the Highest Revenue**

A new sheet was created containing **only the destination names and total revenue**.

To find the **destination with the highest revenue**, the following Excel functions were used:

- **Finding the maximum revenue:**
- **Finding the corresponding destination:**

This identified the destination that generated the highest revenue.

![high rvenue des 1.png](Flight%20Revenue%20Analysis%20Report%2018c4799bb267808eb79ae64d3557d1ed/high_rvenue_des_1.png)

![high rvenue des 2.png](Flight%20Revenue%20Analysis%20Report%2018c4799bb267808eb79ae64d3557d1ed/high_rvenue_des_2.png)

![high rvenue des 3.png](Flight%20Revenue%20Analysis%20Report%2018c4799bb267808eb79ae64d3557d1ed/high_rvenue_des_3.png)

---

### **3. Analyzing Revenue by Seating Class**

Another sheet was created to analyze revenue based on different seating classes.

![seating class 1.png](Flight%20Revenue%20Analysis%20Report%2018c4799bb267808eb79ae64d3557d1ed/seating_class_1.png)

![seating class 2.png](Flight%20Revenue%20Analysis%20Report%2018c4799bb267808eb79ae64d3557d1ed/seating_class_2.png)

![seating class 3.png](Flight%20Revenue%20Analysis%20Report%2018c4799bb267808eb79ae64d3557d1ed/seating_class_3.png)

- This sheet contained only the **destinations and revenues from First Class, Business Class, and Economy Class**, **excluding cargo revenue**.
- The **SUM function** was used across the columns to calculate total revenue for each seating class:
- These formulas were dragged down the table to apply to all destinations.

---

## **Preparing Data for Visualization in Tableau**

After calculating the necessary KPIs, a new **summary table** was created containing the key values needed for visualization in **Tableau**.

![new summary table.png](Flight%20Revenue%20Analysis%20Report%2018c4799bb267808eb79ae64d3557d1ed/new_summary_table.png)

This structured data was then imported into **Tableau** for visual representation.

---

# **Data Visualization in Tableau**

The following visualizations were created in **Tableau** to provide clear insights into the dataset:

[public.tableau.com](https://public.tableau.com/app/profile/tiffany.nwanne/viz/FlightsRevenueAnalysis/Dashboard1)

1. First Class Revenue from all destinations
2. Business Class Revenue from all destinations
3. Economy Class Revenue from all destinations
4. Cargo Revenue from all destinations

---

# Recommendations

### **1. Increase Focus on Economy Class Revenue**

The analysis revealed that Economy Class generates the highest revenue among all seating categories. This indicates strong passenger demand for budget-friendly travel options. To maximize this revenue stream, the airline should consider expanding Economy Class capacity on high-demand routes. Additionally, offering bundled packages that include baggage, priority boarding, and in-flight meals can increase per-passenger revenue. A loyalty program tailored to frequent Economy Class travelers could also encourage repeat bookings and enhance customer retention.

### **2. Improve Cargo Revenue Strategy**

While passenger revenue dominates overall earnings, cargo revenue remains a valuable yet underutilized income stream. The analysis showed that PDX (Portland) had the highest cargo revenue, suggesting strong freight demand on that route. To capitalize on this, the airline should explore increasing cargo capacity on high-demand routes. Partnering with logistics and e-commerce companies can further drive cargo bookings, ensuring consistent utilization of available freight space. Additionally, offering discounts for bulk shipments or promotional pricing during off-peak hours could attract more businesses to use the airline's cargo services.

### **3. Optimize Route Planning for Revenue Maximization**

The destination with the highest total revenue was SEA (Seattle), indicating a strong passenger flow and demand for flights to that location. To leverage this, the airline should consider increasing the frequency of flights to SEA and other high-revenue destinations. Furthermore, introducing premium services such as luxury lounges, priority boarding, and flexible ticket options for these routes could enhance the travel experience and justify higher ticket prices. Conducting further analysis to identify similar underutilized profitable routes can also help the airline optimize its network and allocate resources more effectively.

### **4. Improve Business Class Performance**

The data showed that Business Class revenue lags behind Economy Class, highlighting an opportunity for improvement. To boost Business Class performance, the airline should focus on targeted marketing efforts, particularly toward corporate travelers and frequent flyers. Offering last-minute upgrade incentives at discounted rates can help fill empty seats while increasing revenue. Enhancing Business Class perks, such as improved in-flight meals, access to exclusive lounges, and expedited check-in services, can also attract high-paying customers who prioritize comfort and convenience.

### **5. Use Data-Driven Pricing Strategies**

Implementing a dynamic pricing model can significantly enhance revenue by adjusting ticket prices based on demand fluctuations. The airline can increase ticket prices during peak travel seasons when demand is high and offer competitive discounts during off-peak periods to maximize seat occupancy. Early-bird promotions can encourage advance bookings, ensuring stable revenue flow, while last-minute deals can help fill remaining seats before departure. By leveraging real-time data on booking trends and customer behavior, the airline can optimize pricing strategies and improve profitability.

### **6. Improve Data-Driven Decision Making**

To sustain long-term revenue growth, the airline should integrate data analytics into its decision-making processes. Tableau dashboards should be utilized for real-time revenue tracking, helping management identify trends and make informed business adjustments. Conducting monthly revenue performance reviews can highlight areas of improvement, such as adjusting flight schedules, reallocating aircraft to high-performing routes, and modifying ticket pricing strategies. Furthermore, predictive analytics can be used to forecast demand patterns, allowing the airline to proactively adjust operations to meet market needs and maximize profitability.

By implementing these recommendations, the airline can enhance revenue generation, optimize resource allocation, and improve customer satisfaction, ensuring a competitive edge in the aviation industry

# Conclusion

This analysis revealed a total revenue of **$838,000**, with **Economy Class as the highest revenue generator**, **SEA (Seattle) as the top revenue-producing destination**, and **PDX (Portland) leading in cargo revenue**, highlighting key opportunities for optimizing route planning, seating class performance, and cargo operations through data-driven strategies.