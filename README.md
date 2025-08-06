# Retail Data Mining for Inventory Optimization and Sales Growth

## 1. Project Overview
This project applies data mining and machine learning to a large-scale retail sales dataset to optimize inventory management and increase sales. The analysis extracts purchasing patterns, customer segments, and actionable insights to support smarter business decisions.

## 2. Dataset
- **Name:** Retail Sales Dataset
- **Source:** [Kaggle Retail Sales Dataset](https://www.kaggle.com/datasets/mohammadtalib/retail-sales-dataset)
- **Size:** 100,000+ transactions, multi-store simulation
- **Main attributes:**
    - Transaction_ID, Date, Product_Category, Product_Brand
    - Quantity, Amount
    - Customer demographics (ID, Gender, Age, Country, City)
    - Ratings, Feedback
    - Payment_Method, Shipping_Method
    - Order_Status

## 3. Data Preprocessing
- Remove irrelevant/duplicate columns (e.g., ad_id, zipcode)
- Handle missing values (median for numerics, 'Unknown' for categoricals)
- Normalize/cross-fill related fields (e.g., Feedback ↔ Ratings, City ↔ Country)
- Convert date formats, generate time features (Month, Quarter, Weekday)
- Feature engineering (e.g., Total_Amount = Quantity × Amount)

## 4. Exploratory Data Analysis (EDA)
- Revenue trends by month, week, product category, city
- Analyze customer segments by age, gender, and loyalty
- Visualize sales distributions, best-selling products, payment methods
- Detect seasonality and anomalies in sales data

## 5. Machine Learning & Analytics
- **Basket Analysis (Apriori):** Discover product association rules, support cross-selling strategies
- **Customer Segmentation (KMeans, RFM):** Identify high-value and targetable customer groups
- **Inventory Optimization:** Analyze demand vs. reorder points, suggest inventory policy improvements
- **Sales Forecasting (Prophet):** Predict future revenue trends for planning

## 6. Results & Insights
- Key findings: Water, Smartphones, and Fiction are top sellers; Friday is peak sales day
- Strong product bundles detected (Boots & Oxfords/Sneakers, beverage combos)
- Customer clusters revealed high-value vs. price-sensitive groups
- Inventory levels generally set above demand for safety, with optimization recommendations
- Prophet modeling highlighted clear weekly/seasonal cycles in sales

## 7. Limitations & Future Work
- Data only covers ~1 year; need multi-year data for deeper trends
- Explore advanced forecasting (ARIMA, LSTM) and product recommendation engines
- Add more real-time dashboards and business KPIs

## 8. How to Run / Usage
**Requirements:** Python 3.x, pandas, numpy, matplotlib, seaborn, scikit-learn, mlxtend, Prophet  
**Example usage:**
```bash
python preprocess.py
python eda.py
python basket_analysis.py
python customer_segmentation.py
python forecast.py
```
## 9. Team & Credits

**Team 2 – Samsung Innovation Campus Big Data Capstone (July 2025)**

| Name                  | Role/Contribution                                                   |
|-----------------------|---------------------------------------------------------------------|
| Trương Thái Bảo       | Team leader, project objectives, data cleaning, basket analysis, data visualization |
| Nguyễn Đào Hồng Như   | Revenue forecasting (Prophet), EDA, trend visualization, report writing |
| Nguyễn Văn Tú         | Data processing, action plan, supporting analyses                   |
| Nguyễn Lư Hồng Phương | Data cleaning, model result summary, RFM analysis                   |
| Nguyễn Kim Vương Ý    | Data standardization, customer segmentation, model validation, inventory optimization, reporting |




