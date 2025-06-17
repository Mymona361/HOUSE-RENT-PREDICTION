🏠 House Price Prediction Using Linear Regression

This is a simple Python project that uses Linear Regression to predict house prices based on their area (in square feet). The model is trained using sample data and allows user input to predict the price of a house.

📌 Features
Uses scikit-learn for linear regression

Takes user input for house area

Predicts and displays the estimated house price

🛠 Technologies Used
Python 3

pandas

scikit-learn


 📊 Sample Data

The training data used is hardcoded as follows:

| Area (sqft) | Price (Tk) |
| ----------- | ---------- |
| 1000        | 20000      |
| 1500        | 30000      |
| 2000        | 40000      |
| 2500        | 50000      |
| 3000        | 60000      |


 🚀 How It Works

1. The script creates a DataFrame using `pandas`.
2. A `LinearRegression` model is trained on the data.
3. The user is prompted to input the area of a house.
4. The model predicts the price based on the provided area.
5. The predicted price is printed in a formatted output.



 🛠 Requirements

To run the script, make sure you have the following Python packages installed:

```bash
pip install pandas scikit-learn
```



 🧾 Usage

Run the script using a Python interpreter:

```bash
python house_price_predictor.py
```

You'll be prompted to enter the area of the house:

```
Enter the area of the house in square feet:
2200
```

Output:

```
predicted price: Tk 44,000.00
predicted price: Tk 44,000
```

---

 📁 Code Summary

```python
from sklearn.linear_model import LinearRegression
import pandas as pd

data = {
    'Area': [1000, 1500, 2000, 2500, 3000],
    'Price': [20000, 30000, 40000, 50000, 60000]
}

df = pd.DataFrame(data)

x = df[['Area']]
y = df['Price']

model = LinearRegression()
model.fit(x, y)

area = float(input("Enter the area of the house in square feet: \n"))
predicted_price = model.predict([[area]])

print(f"predicted price: Tk {predicted_price[0]:,.2f}")
print(f"predicted price: Tk {int(predicted_price[0]):,}")
```

---



