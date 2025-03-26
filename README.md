![image_alt](https://github.com/etimexo/Hotel_booking_analysis/blob/main/visualizations/pexels-pixabay-258154%20(1).jpg)
![pexels-pixabay-258154 (1)](https://github.com/user-attachments/assets/cd15db27-d71a-435b-bd5d-e4158bd7ae65)

# Hotel_booking_analysis
## 📌 Project Overview

This project analyzes hotel booking data to uncover insights related to booking requests, pricing, room types, and customer preferences. The goal is to identify patterns that can help optimize pricing strategies and improve customer experience.

📊 Dataset Description

The dataset contains information about hotel bookings, including:
1. Booking requests and special requests
2. Room types and their prices
3. Monthly booking trends
4. Special requests and their impact on pricing
Image of the raw data:
![image_alt](https://github.com/etimexo/Hotel_booking_analysis/blob/main/visualizations/raw_data.png)
___

##🛠 Data Processing

Data Cleaning: There wasn't much to do here as the dataset was from Kaggle. But what I did do was to create another column named "arrival_month_abc".
This was because the original months in the data were numeric and I needed their alphabetic representations for visualization.
![image_alt](https://github.com/etimexo/Hotel_booking_analysis/blob/main/visualizations/month_formula.png)

Feature Engineering: Created additional features like month-wise analysis.

Visualization: Used charts and graphs to explore trends.
___

## 📈 Exploratory Data Analysis (EDA)

Below are key insights from the analysis:

### 1️⃣ Booking Requests Trend

This visualization shows the total number of bookings by request type.


📌 Include booking_by_requests.png here.

2️⃣ Monthly Booking Trends

Displays how bookings vary across different months.

📌 Include month.png here.

Formula used for month extraction: *Include *month_formula.png

3️⃣ Pricing Analysis

Price per Room Type: Understanding how different room types are priced.

📌 Include price_per_room_type.png here.

Price based on Special Requests: Analyzing how special requests affect pricing.

📌 Include price_per_special_requests.png here.

4️⃣ Room Type Preferences

Examines which room types are booked the most.

📌 Include room_type.png here.

📝 Key Findings & Insights

Room pricing varies significantly based on type and special requests.

Certain months have peak booking seasons.

Special requests influence pricing and booking trends.

📂 Repository Structure

📂 Hotel-Booking-Analysis
│── 📁 data/              # Raw & processed datasets
│── 📁 visuals/           # Charts and graphs
│── 📄 analysis.ipynb     # Jupyter Notebook with code & insights
│── 📄 README.md         # Project documentation

🔮 Future Improvements

Incorporate machine learning to predict booking cancellations.

📌 Author

Elijah Obisesan Timilehin
