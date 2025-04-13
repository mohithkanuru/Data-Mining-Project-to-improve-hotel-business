# Using Data Mining to Improve Hotel Business

## Overview

This project was undertaken as part of the CSL-515: Data Mining and Warehousing course under the guidance of Prof. Durga Toshniwal. The goal is to utilize data mining techniques to gain insights into hotel booking behavior and customer reviews to ultimately improve hotel business operations and customer satisfaction.

## Team Members

- Varre Tejaswini (21114109)
- Uppala Vivek Narayan (21114108)
- Male Jithendra (21114055)
- Chiranjan Kumarr K S (21114033)
- Sapavath Yashwanth Krishna Naik (21114093)
- Kanuru Mohith Kumar Reddy (21114047)

## Datasets Used

1. **Hotel Booking Dataset** – Contains records of hotel reservations with features such as lead time, customer type, market segment, booking status, and more.
2. **TripAdvisor Reviews Dataset** – Contains customer reviews and ratings for hotels, used for classification tasks (sentiment analysis and rating prediction).

## Methodology

### Data Preprocessing
- Removed null and duplicate entries.
- Normalized and encoded categorical variables.
- Merged datasets wherever necessary for enhanced analysis.

### Exploratory Data Analysis (EDA)
- Analyzed booking trends by month, country, and hotel type.
- Investigated cancellation patterns and their relation to lead time, customer type, etc.
- Explored the impact of special requests, repeated guests, and distribution channels.

### Clustering and Segmentation
- Applied KMeans clustering to segment customers based on their booking behaviors.
- Identified patterns in cluster profiles such as business vs leisure travelers.

### Association Rule Mining
- Extracted frequent patterns and itemsets to find relationships between features like special requests, room type, and cancellations.

### Sentiment Analysis and Rating Prediction
- Data Prep: Cleaned and labeled review data, then split into train, val, and test sets.
- Modeling: Fine-tuned a pretrained transformer (e.g., DistilBERT) for sentiment and rating prediction.
- Training: Used Hugging Face Trainer with GPU, mixed-precision, and learning rate scheduling.
- Evaluation: Logged detailed metrics (accuracy, precision, recall, F1) after each epoch.

## Insights from the Analysis

### Booking Behavior

- **Customer Preferences**: Different nationalities and market segments exhibit distinct booking habits. City hotels are favored by international travelers while resort hotels attract domestic tourists.
- **Lead Time Analysis**: Longer lead times often correlate with higher cancellation rates. Hotels can tailor cancellation policies or reminders accordingly.
- **Loyal Customers**: Repeat guests have higher stay durations and lower cancellation rates, emphasizing the value of loyalty programs.

### Impact of Cancellations

- **Cancellation Rates**: A noticeable number of bookings are canceled, particularly those made online or far in advance. This affects revenue and planning.
- **Temporal Variation**: Cancellations vary with season and month. High cancellation rates in off-seasons offer room for flexible pricing strategies.

### Sentiment Analysis of Reviews

- **Positive Sentiments**: Guests appreciated hotel location, cleanliness, and friendly staff.
- **Negative Sentiments**: Complaints centered around slow service, room readiness, and check-in delays.
- **Emotional Cues**: Emotions like joy and trust were dominant in positive reviews, while anger and sadness surfaced in negative ones.

### Service Recommendations and Business Improvements

- **Targeted Offers**: Personalized deals based on customer segment and booking channel can improve conversion rates.
- **Overbooking Strategy**: Data-driven overbooking in low-risk segments during peak seasons can minimize lost revenue.
- **Operational Focus**: Investing in staff training and front-desk efficiency can address common review concerns.

### Clustering and Customer Segmentation

- **Guest Segmentation**:
  Helps hotels send the right messages and offers to different types of guests.
  Improves planning by assigning suitable rooms and services based on guest needs.

- **Pricing Strategy**:
  Allows flexible pricing by understanding how much each guest type is willing to pay.
  Helps offer the right deals like discounts or premium packages to the right guests.

- **Booking Behaviour Patterns**:
  Lets hotels reduce cancellations and no-shows with smart reminders and options.
  Boosts bookings and guest satisfaction through timely, personalized offers.


## Conclusion

This project highlights how data mining techniques such as clustering, association rule mining, and sentiment analysis can be used effectively to understand customer behavior and enhance hotel business strategies. These insights can help hotels in targeted marketing, service improvements, and operational efficiency.
