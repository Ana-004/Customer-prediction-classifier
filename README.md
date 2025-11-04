# Customer-prediction-classifier
This project performs customer subscription prediction using the Bank Marketing dataset. It involves data preprocessing, encoding categorical features, normalization, and model training using the Gaussian Naive Bayes classifier to predict whether a customer will subscribe to a term deposit.

# Goal
The goal is to help financial institutions identify potential customers who are likely to subscribe, improving marketing efficiency and decision-making.

## Technologies Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn

## Details of the Dataset columns
*Bank client data:*

1 - age (numeric)

2 - job : type of job (categorical: "admin.","unknown","unemployed","management","housemaid","entrepreneur","student","blue-collar","self-employed","retired","technician","services")

3 - marital : marital status (categorical: "married","divorced","single"; note: "divorced" means divorced or widowed)

4 - education (categorical: "unknown","secondary","primary","tertiary")

5 - default: has credit in default? (binary: "yes","no")

6 - balance: average yearly balance, in euros (numeric)

7 - housing: has housing loan? (binary: "yes","no")

8 - loan: has personal loan? (binary: "yes","no")

*Related with the last contact of the current campaign:*

9 - contact: contact communication type (categorical: "unknown","telephone","cellular")

10 - day: last contact day of the month (numeric)

11 - month: last contact month of year (categorical: "jan", "feb", "mar", …, "nov", "dec")

12 - duration: last contact duration, in seconds (numeric)

*Other attributes:*

13 - campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)

14 - pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric, -1 means client was not previously contacted)

15 - previous: number of contacts performed before this campaign and for this client (numeric)

16 - poutcome: outcome of the previous marketing campaign (categorical: "unknown","other","failure","success")

*Output variable (desired target):*

17 - y - has the client subscribed a term deposit? (binary: "yes","no").

## Steps Performed
1. **Data Collection**
   - Imported dataset (`bank-marketing.xlsx`) using Google Colab.
2. **Data Preprocessing**
   - Handled missing values using forward fill.
   - Encoded categorical variables using One-Hot Encoding.
   - Normalized numerical features with `StandardScaler`.
3. **Model Training**
   - Split data into training and test sets (80-20).
   - Trained a **Gaussian Naive Bayes (GNB)** model.
4. **Evaluation**
   - Evaluated model performance using **accuracy score**, **classification report**, and **confusion matrix**.

## How to Run
1. Upload `bank-marketing.xlsx` to Google Colab.
2. Run all cells in the notebook `customer-prediction-classification.ipynb`.
3. View results and confusion matrix plots at the end.

## Results
- **Model Accuracy:** ~87.9%
- The GNB model shows good predictive performance on test data.
