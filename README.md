# HOTEL BOOKING ANALYSIS
![image_alt](https://github.com/etimexo/Hotel_booking_analysis/blob/main/images/hotel1.png)

## 📌 Project Overview

This project analyzes hotel booking data to uncover insights related to booking requests, pricing, room types, and customer preferences. The goal is to identify patterns that can help optimize pricing strategies and improve customer experience.

## 📊 Dataset Description
This dataset was gotten from [Kaggle](https://www.kaggle.com/datasets/ahsan81/hotel-reservations-classification-dataset)

The dataset contains information about hotel bookings, including:
1. Booking requests and special requests
2. Room types and their prices
3. Monthly booking trends
4. Special requests and their impact on pricing
Image of the raw data:

![image_alt](https://github.com/etimexo/Hotel_booking_analysis/blob/main/images/rawData.png)
___

## 🛠 Data Processing

Data Cleaning: There wasn't much to do here as the dataset was from Kaggle. But what I did do was to create another column named "arrival_month_abc".
This was because the original months in the data were numeric and I needed their alphabetic representations for visualization.

![image_alt](https://github.com/etimexo/Hotel_booking_analysis/blob/main/images/monthFormula.png)

Feature Engineering: Created additional features like month-wise analysis.

Visualization: Used charts and graphs to explore trends.
___

## 📈 Exploratory Data Analysis (EDA)

Below are key insights from the analysis:

### 1️⃣ Booking Requests Trend

This visualization shows the total number of bookings by request type.

![image_alt](https://github.com/etimexo/Hotel_booking_analysis/blob/main/images/bookingStatus.png)

2️⃣ Monthly Booking Trends

Displays how bookings vary across different months.

![Screenshot 2025-04-09 104549](https://github.com/user-attachments/assets/d3575233-6d8a-4ad9-8c82-89cf6c447ddd)


Formula used for month extraction: *Include *month_formula.png

3️⃣ Pricing Analysis

Price per Room Type: Understanding how different room types are priced.

![image_alt](https://github.com/etimexo/Hotel_booking_analysis/blob/main/images/pricePerRoomType.png)

Price based on Special Requests: Analyzing how special requests affect pricing.

![image_alt](https://github.com/etimexo/Hotel_booking_analysis/blob/main/images/pricePerSpecial.png)

4️⃣ Room Type Preferences

Examines which room types are booked the most.

![Screenshot 2025-04-09 104655](https://github.com/user-attachments/assets/1f196ca1-dba2-4a5c-8bb7-7cf8b2d1b06e)


___
## 📝 Key Findings & Insights

Room pricing varies significantly based on type and special requests.
Certain months have peak booking seasons.
Special requests influence pricing and booking trends.
Below is the revenue generated on all bookings and the amount not generated due to cancelations:

![image](https://github.com/user-attachments/assets/43d9f0ca-d359-4c75-820b-a3400f9c4781)

___

#### Slicers were added to the charts to explore relationships between different variables. These slicers include whether a customer is a repeat guest and whether they require a parking space. Both factors were observed to influence the customer's booking status—whether they successfully completed the booking or later canceled.

![Screenshot 2025-04-09 105418](https://github.com/user-attachments/assets/7b4e7181-410c-4eb1-9246-79640c8a08a3)

![image_alt]![Screenshot 2025-04-09 105418](https://github.com/user-attachments/assets/ea2db9cd-33bc-483a-8018-2cb351478961)

![Screenshot 2025-04-09 105532](https://github.com/user-attachments/assets/fd757c74-bbdc-4334-a406-1b06e34bd5d1)


___

# Recommendations
Based on the insights gained from the analysis, the following recommendations can be made to improve customer retention, optimize pricing strategies, and reduce cancellations:
## 1. Enhance Loyalty Programs for Repeat Guests
Since repeat guests tend to have a significant influence on booking trends, offering targeted discounts or exclusive perks could encourage more frequent stays and increase retention rates.

## 2. Improve Parking Availability
The analysis showed that the availability of parking space affects booking decisions. Hotels should ensure sufficient parking options or provide alternative solutions (e.g., partnerships with nearby parking lots) to attract customers who require this service.

## 3. Optimize Room Pricing Strategy
The pricing analysis across room types and special requests suggests that adjusting pricing dynamically based on demand and customer preferences could increase revenue. Implementing data-driven pricing strategies will help maximize occupancy rates.

___

## Model Development Process
I went further to build a classification model to predict whether a customer would cancel their hotel booking using historical booking data. The target variable used for prediction was booking_status_Not_Canceled (1 = Not Canceled, 0 = Canceled).

### Steps Taken:
- Applied one-hot encoding to categorical features (type_of_meal_plan, room_type_reserved, market_segment_type, and booking_status).
- Split the dataset into training (80%) and testing (20%) sets.
-Model Selection & Training:
Evaluated three different models: Logistic Regression, Decision Tree Classifier and Random Forest Classifier
- Used default hyperparameters for initial training.

### Model Evaluation:
Random Forest performed best, achieving 90.5% accuracy, followed by Decision Tree (86.9%) and Logistic Regression (79.5%).
Performance metrics such as precision, recall, and F1-score were analyzed to compare results with appropriate visualizations in the [Jupyter notebook](https://github.com/etimexo/Hotel_booking_analysis/blob/main/hotel_booking.ipynb)

Insights from Results:
- Booking behavior impacts cancellations: Features like lead time, previous cancellations, and special requests play a major role in predicting cancellations.
- Market segment influences cancellation trends: Corporate and online bookings exhibit different cancellation behaviors.
- Random Forest is the most effective model: It captures complex patterns in customer behavior, making it the best choice for prediction.
- Decision Tree risks overfitting: It learns the training data well but may not generalize as effectively.
- Logistic Regression struggles with complex relationships: Since cancellations are influenced by multiple factors in a non-linear way, this model has lower performance.

You can view the whole process [here](https://github.com/etimexo/Hotel_booking_analysis/blob/main/hotel_booking.ipynb)
___

# Conclusion
This analysis provided valuable insights into customer booking behaviors, pricing trends, and factors influencing cancellations. Key findings include the impact of repeat guests and parking space availability on booking status, as well as variations in room pricing and special requests. By leveraging these insights, hotels can optimize pricing strategies, improve customer experience, and reduce booking cancellations.

Implementing targeted marketing strategies and customer-focused policies will ultimately help hotels increase revenue, enhance customer satisfaction, and build long-term customer loyalty. Future work could involve deeper predictive modeling to forecast cancellations and demand trends more accurately.

___

# 📌 Author

### Elijah Obisesan Timilehin
### [LinkedIn Profile](https://www.linkedin.com/in/teoso)
### [Send me a mail](elijahobisesan01@gmail.com)
