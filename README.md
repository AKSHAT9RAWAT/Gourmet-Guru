# Gourmet Guru - Food Ordering and Recommendation System

This project consists of two Android applications inspired by the food ordering systems used in Chinese restaurants:

- **User Application:** Gourmet User
- **Manager Application:** Gourmet Manager

## 1. Gourmet User

### Overview

Gourmet User is designed to provide a fast and convenient way for users to order food and drinks while leveraging a machine learning model to recommend food based on customer feedback. The project includes three major components:

1. **Sentiment Analysis:** Utilizing an RNN model to analyze customer feedback.
2. **ML Model Integration:** Incorporating the machine learning model into the Android application.
3. **Food Item Ranking:** Ranking menu items based on customer reviews.

### Sentiment Analysis with RNN

- **Dataset:** Amazon food review dataset
  - **Training:** 300,000 reviews
  - **Testing:** 100,000 reviews
- **Accuracy:** 
  - Training: ~93%
  - Testing: ~91%
- **Model:** tf.Keras model converted to tflite for Android integration
- **Functionality:** Performs sentiment analysis on user reviews to generate a score for each dish.

### Application Workflow

1. **Login:** User logs into the application.
2. **Scan QR Code:** User scans the QR code at the restaurant table.
3. **Select Food:** User selects desired dishes from the menu.
4. **Checkout:** User proceeds to checkout.
5. **Payment:** Payment is processed via Paytm gateway.
6. **Order Confirmation:** Restaurant manager/chef receives and confirms the order.
7. **Give Review:** User provides feedback on their order.
8. **Review Result:** Feedback is analyzed, and the food score is updated.

### Key Features

- **Payment Gateway:** Paytm integration for seamless transactions.
- **Machine Learning:** Tflite RNN model for sentiment analysis.
- **Firebase:** Authentication, Realtime Database, and Storage for secure and efficient data management.
- **Image Handling:** Glide for image loading, Image Compressor, and Cropper.
- **QR Code Scanner:** For easy table identification and order placement.

### Food Score System

- **Review Analysis:** Each review contributes to the score of the respective dish.
- **Menu Sorting:** Dishes with higher scores are displayed at the top of the menu.

## 2. Gourmet Manager

### Overview

Gourmet Manager is designed for restaurant managers. It provides notifications for new orders and allows managers to confirm orders once they are served, enabling users to provide feedback.

### Key Features

- **Order Management:** Managers receive and confirm orders.
- **Notification System:** Alerts for new orders.
- **User Feedback:** Enables the feedback mechanism for user reviews.

### Technologies Used

- **Payment Gateway:** Paytm
- **Machine Learning:** Tflite RNN model
- **Firebase:** Authentication, Realtime Database, Storage
- **Image Handling:** Glide, Image Compressor, Cropper
- **Networking:** Volley for network operations
- **QR Code Scanner:** For table identification and order placement

## Conclusion

Gourmet Guru, with its Gourmet User and Gourmet Manager applications, provides a robust, efficient, and user-friendly food ordering and recommendation system. By integrating advanced machine learning models for sentiment analysis and offering seamless payment and feedback mechanisms, these applications aim to enhance the dining experience for both customers and restaurant managers.

