# Bank Marketing Campaign Prediction by Nesly Cesar

## Project Overview
This project aims to improve the effectiveness of bank marketing campaigns by predicting client subscriptions to term deposits. Using a dataset from a Portuguese banking institution, predictive modeling techniques were applied to identify the key factors influencing subscription decisions and to develop a model that can accurately forecast client behavior. The final model, a **Tuned Gradient Boosting Classifier**, was selected for its performance in balancing precision and recall, making it the most effective at predicting client subscriptions.

## Objectives
1. **Improve campaign success**: Apply predictive modeling techniques to identify clients most likely to subscribe to a term deposit.
2. **Identify key factors**: Determine which features (e.g., call duration, previous campaign success) most significantly influence client decisions.
3. **Model comparison**: Compare several machine learning models to find the most accurate one for predicting term deposit subscriptions.
4. **Optimize marketing strategies**: Use insights gained from data mining to enhance marketing effectiveness.

## Dataset
The dataset contains information from marketing campaigns conducted by a Portuguese bank. It includes client-related attributes (e.g., age, job), marketing campaign data (e.g., number of contacts, duration), and the target variable (`y`), which indicates whether the client subscribed to a term deposit.

- **Number of Instances**: 45,211
- **Number of Features**: 16 input features + 1 target variable (`y`)

### Key Features:
- **Call Duration**: Length of the last call in the campaign.
- **Previous Campaign Outcome**: Outcome of the client’s previous campaign interaction.
- **Age**: Client's age.
- **Balance**: Average yearly balance of the client.
- **Housing Loan**: Whether the client has a housing loan or not.

## Final Model: Tuned Gradient Boosting Classifier
The final model chosen for this project is a **Tuned Gradient Boosting Classifier**, optimized for its balance between precision and recall. The model was fine-tuned using GridSearchCV to find the best hyperparameters for learning rate, number of estimators, and max depth.

### Performance Metrics:
- **Accuracy**: 90.08%
- **F1 Score**: 0.476
- **Precision**: 0.623
- **Recall**: 0.386

## Key Insights
- **Call Duration** is the most important factor, with longer calls indicating a higher likelihood of subscription.
- Clients with **previous successful campaign outcomes** are more likely to subscribe again.
- Clients **without housing loans** show a higher subscription rate, likely due to greater financial flexibility.
- **Age and Balance** are significant factors, with older clients and those with higher balances more likely to subscribe.

## Project Structure

```plaintext
├── data/
│   └── bank_full.csv         # The dataset used for the project
├── notebooks/
│   └── Bank Marketing Strategies complete notebook.ipynb  # All processes (Data wrangling, EDA, Feature preprocessing, etc.) notebook
├── reports/
│   └── final_model_metrics.txt    # Text file with final model performance and features
│   └── Capstone_Final_Report.docx # Project Report
├── README.md                      # This ReadMe file
