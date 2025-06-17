
🏠 House Price Prediction Using Linear Regression

This is a simple Python project that uses Linear Regression to predict house prices based on their area (in square feet). The model is trained using sample data and allows user input to predict the price of a house.

📌 Features

Uses scikit-learn for linear regression

Takes user input for house area

Predicts and displays the estimated house price



📈 Sample Dataset

Area (sqft)	Price (Tk)

1000	20000
1500	30000
2000	40000
2500	50000
3000	60000


🚀 How to Run

1. Clone this repository

git clone https://github.com/your-username/house-price-prediction.git
cd house-price-prediction


2. Install Dependencies

pip install pandas scikit-learn


3. Run the Script

python house_price_predictor.py


4. Enter the area when prompted (e.g., 2200) and get the predicted price.




---

🧠 How It Works

A LinearRegression model is trained on a small dataset of house areas vs. prices.

The model learns the relationship (price per square foot).

The user provides the area, and the model predicts the corresponding price.



---

📋 Example Output

Enter the area of the house in square feet:
2200
predicted price: Tk 44,000.00
predicted price: Tk 44,000


---

📄 License

This project is open-source and available under the MIT License.


---

Let me know if you want me to add a .gitignore, LICENSE file, or convert this into a Jupyter Notebook format as well.
