# Zomato-Data-Analysis--SQL

### 📊 Data Exploration and Analysis using SQL Server

This project focuses on exploring and analyzing the Zomato dataset using SQL. Zomato is a leading Indian multinational restaurant aggregator and food delivery company. The goal of this analysis is to gain insights into their operations and restaurant listings.

---

## 📁 Dataset Overview

The dataset contains over **9000 records** with features such as:
- `Restaurant_ID`
- `Restaurant_Name`
- `City`
- `Location`
- `Cuisines`
- `Country_Code`
- and other restaurant-related details.

---

## 🛠️ Data Exploration Tasks

Using SQL Server, the following steps were taken during data exploration:

1. Reviewed table schema including column names, data types, and constraints.
2. Checked and removed duplicate values in the `Restaurant_ID` column.
3. Dropped irrelevant/unwanted columns to clean the dataset.
4. Merged two different tables and added the `Country_Name` using `Country_Code` as the primary key.
5. Identified and corrected misspelled city names.
6. Counted the number of restaurants using rolling/moving count (window functions).
7. Computed min, max, and average for `Votes`, `Rating`, and `Currency`.
8. Created a new categorical column for ratings.

---

## 🔍 Key Insights from the Analysis

1. **90.67%** of restaurants in the dataset are located in **India**, followed by **USA (4.45%)**.
2. Only **2 out of 15 countries** offer online delivery:
   - **28.01%** of Indian restaurants
   - **46.67%** of UAE restaurants
3. The dataset is heavily India-centric, so further insights focus on Indian restaurants.
4. **Connaught Place (New Delhi)** has the highest number of restaurant listings (122), followed by **Rajouri Garden (99)** and **Shahdara (87)**.
5. Most popular cuisine in Connaught Place is **North Indian**.
6. Out of 122 restaurants in Connaught Place, only **54** offer table booking.
7. Average rating:
   - With table booking: **3.9/5**
   - Without table booking: **3.7/5**
8. The best **moderately priced** Indian restaurant based on:
   - Average cost for two < 1000
   - Rating > 4
   - Votes > 4
   - Offers both table booking and online delivery

   is **"India Restaurant"** in **Kolkata, India** (`Restaurant_ID: 20747`).

---

## 🧠 Tools & Technologies Used
- **SQL Server**
- **SQL (DDL, DML, Window Functions, Joins, Aggregations)**

---

## 📌 Conclusion

This project demonstrates how SQL can be used for end-to-end data exploration and business insight generation. The analysis highlights patterns in customer services, geographical distribution, and restaurant quality metrics that can help Zomato and similar businesses make informed decisions.

---

