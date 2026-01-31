🍔 Food Delivery Data Analysis – Hackathon Project
📌 Project Overview

This project focuses on analyzing a food delivery platform dataset by integrating data from multiple sources such as orders, users, and restaurants. The goal is to extract meaningful business insights like customer behavior, revenue distribution, and membership-based analysis using Python and Pandas.

The project was developed as part of a hackathon, emphasizing real-world data handling and analysis.

📂 Dataset Description

The following datasets were used:

orders.csv
Contains transactional order data such as order ID, user ID, restaurant ID, total amount, etc.

users.json
Contains user details including membership type (Gold/Regular), city, and user identifiers.

restaurants.sql
Restaurant metadata (not directly used due to SQL format).

merged_data.csv ✅
A pre-merged and cleaned dataset combining orders and users, used for final analysis.

🛠️ Technologies Used

Python 🐍

Pandas

Jupyter Notebook

Git & GitHub

📊 Key Analysis Performed

Data loading and inspection

Handling missing values

Filtering Gold members

Revenue analysis by city

Grouping and aggregation using Pandas

▶️ How to Run the Project
1️⃣ Clone the repository
git clone https://github.com/your-username/food-delivery-analysis.git
cd food-delivery-analysis

2️⃣ Open Jupyter Notebook
jupyter notebook

3️⃣ Load the merged dataset
import pandas as pd

df = pd.read_csv("merged_data.csv")
df.head()

📈 Sample Analysis Code
gold_df = df[df["membership_type"] == "Gold"]

city_revenue = gold_df.groupby("city")["total_amount"].sum()
city_revenue.sort_values(ascending=False)

🏆 Key Insight

The city with the highest total revenue from Gold members was identified using grouped revenue analysis.

⚠️ Notes

The restaurants.sql file was not directly used as SQL parsing is beyond the scope of this hackathon.

Analysis was performed on the already merged dataset (merged_data.csv) to ensure efficiency and accuracy.

👩‍💻 Author

Princy
B.Tech Student | Data Science & Machine Learning Enthusiast
