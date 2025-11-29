# 🏦 Banking Transaction Analysis
- Exploratory Data Analysis (EDA) | Fraud Detection | User Spending Behaviour

- This project performs a detailed analysis of Banking Transactions using a realistic dataset containing 15,000+ records of payments, merchants, users, categories, transaction types, and fraud labels.

- The goal of this project is to understand:

- Spending behaviour of users

- Merchant-wise and category-wise spending

- Outlier & anomaly patterns

- Fraud transaction patterns

- Time-based transaction patterns

- Which users & transactions show the highest fraud probability

- The notebook includes EDA, visualizations, insights, and fraud-focused analysis.

- 📁 Project Structure
```
Banking-Transaction-Analysis/
│
├── data/
│   └── Banking.csv                # Transaction dataset
│
├── notebooks/
│   └── BankingTransactionAnalysis.ipynb   # Main EDA notebook
│
├── README.md                      # Project documentation
```

## 📊 Dataset Overview

- The dataset contains 15,000+ bank transactions with the following fields:

  - Column	Description
  - TransactionID	Unique ID of each transaction
  - UserID	User who performed the transaction
  - Date	Timestamp (YYYY-MM-DD HH:MM:SS)
  - TransactionType	UPI / POS / ATM / Online / Card
  - Category	Food, Travel, Bills, Groceries, Shopping, etc.
  - Merchant	Amazon, Uber, Swiggy, PetrolPump, etc.
  - Amount	Transaction value in ₹
  - CardType	Debit or Credit
  - IsFraud	1 = Fraud, 0 = Legitimate

- Fraud patterns were generated using realistic logic:

- Large online payments (> ₹12,000) have higher fraud probability

- 2% background random fraud generation

## 🔍 Key Analysis Performed
### ✅ 1. Data Cleaning

- Checked for null values

- Verified datatypes

- Extracted Date & Time components

- Converted date-time column for analysis

## ✅ 2. Outlier Detection

- Used boxplots to analyze outliers for:

- Categories vs Amount

- Merchants vs Amount

- Transaction Types vs Amount

## ✅ 3. Spending Behaviour

- Average spend by category

- Highest spending merchants

- User-wise spending patterns

- Transaction volume by type

## ✅ 4. Fraud Analysis

- Total fraud count

- Fraud transactions by merchant

- Fraud vs non-fraud amount distribution

- Time-of-day fraud analysis

- User fraud patterns

- Fraud heat map (if added later)

## ✅ 5. Visualizations

- Boxplots

- Bar charts

- Scatter plots

- Countplots

- Time-based charts

## 📈 Insights & Findings (Summary)

- These are some example insights (yours may vary based on notebook):

- Fraud is highest in ONLINE transactions, especially transactions above ₹12,000.

- Certain merchants (like Amazon, IRCTC etc.) show higher high-value transactions → increased fraud checks needed.

- Late-night transactions (11PM – 3AM) have higher fraud percentage.

- Most users spend heavily on Food, Shopping, and Travel.

- Debit cards show lower fraud frequency compared to credit cards.

- Some users repeatedly show suspicious patterns → good candidates for fraud flagging.

- Add your actual insights here once finalized.

## 🚀 How to Run the Project
- Requirements

- Install required libraries:

  - pip install pandas matplotlib seaborn numpy

  - Run the Notebook

  - Clone the repository

  ```
  git clone https://github.com/sAdityas/Banking-Transaction-Analysis.git
  ```

  - Navigate to project folder
  
  ```
  cd Banking-Transaction-Analysis
  ```

  - Launch Jupyter Notebook

  ```
  jupyter notebook
  ```

  - Open the notebook inside notebooks/ folder.

## 🧠 Future Improvements (Roadmap)

- Add correlation heatmap

- Build fraud detection ML model (Logistic Regression / Random Forest)

- Add Power BI dashboard

- Add user segmentation (K-Means)

- Add more detailed time-series analysis

# 👤 Author

## Aditya Sarkale
### 📍 Pune, India
### 🔗 GitHub: @sAdityas
