📦 Food Delivery Data Analysis – Hackathon Project
📌 Project Overview

This project demonstrates how to integrate and analyze data coming from multiple real-world systems using different file formats.
The objective is to combine transactional, user, and restaurant data into a single source of truth and perform meaningful analysis on food delivery orders.

📂 Datasets Used

The project uses three different data sources:

orders.csv

Transactional data

Contains order details such as order ID, user ID, restaurant ID, order date, and total amount

users.json

User master data

Contains user information such as user ID, city, and membership type (Gold / Regular)

restaurants.sql

Restaurant master data

Contains restaurant details such as restaurant ID, cuisine type, and rating

🔄 Data Integration Process

The datasets are combined using LEFT JOINs to ensure all orders are retained.

Join Logic:

orders.user_id → users.user_id

orders.restaurant_id → restaurants.restaurant_id

Why LEFT JOIN?
To retain all order records even if corresponding user or restaurant data is missing.

📁 Final Output

After merging all datasets, a final dataset is created:

final_food_delivery_dataset.csv


This dataset contains:

Order details

User information

Restaurant information

This file acts as the single source of truth for all analysis and questions.

📊 Analysis Performed

Using the final merged dataset, the following analyses were carried out:

Order trends over time

User behavior patterns

City-wise revenue performance

Cuisine-wise revenue contribution

Membership impact (Gold vs Regular users)

Revenue distribution and seasonality

🛠 Tools & Technologies Used

Python

Pandas – data loading, cleaning, merging, and analysis

SQLite – executing SQL file and extracting restaurant data

Jupyter Notebook

GitHub

▶️ How to Run the Project

Place the following files in the same directory as the Jupyter Notebook:

orders.csv

users.json

restaurants.sql

Open the Jupyter Notebook.

Run the cells sequentially.

The final merged file final_food_delivery_dataset.csv will be generated automatically.

✅ Notes

The repository is public for evaluation purposes.

All joins and analysis strictly follow the hackathon instructions.

The final dataset is the only source used to answer MCQs and fill-in-the-blank questions.
