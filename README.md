# 🏡 Real Estate Price Predictor

![Python](https://img.shields.io/badge/Python-3.9-blue.svg)
![Flask](https://img.shields.io/badge/Flask-2.3-lightgrey)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

A machine learning web app that predicts **real estate property prices** based on user inputs like location, square footage, number of bedrooms (BHK), and bathrooms. Built using Flask and a trained regression model, this app helps users estimate property values quickly and accurately.

---

## 🚀 Features

- 🏙️ Predict real estate prices based on inputs
- 📍 Location dropdown auto-populated from data
- 📊 Backend logic powered by regression model
- 🌐 Flask web interface with Bootstrap styling
- 🧠 Model serialized using `joblib`

---

## 🛠 Tech Stack

| Layer        | Technology |
|--------------|------------|
| Backend      | Python, Flask |
| ML Model     | Scikit-learn (Linear Regression or similar) |
| Frontend     | HTML, CSS, Bootstrap |
| Dataset      | Bengaluru house data (CSV) |
| Tools        | Pandas, NumPy, Joblib |

---

## 📂 Project Structure

```
Real-Estate/
├── app.py                 # Flask app entry point
├── model/                 
│   ├── bangalore_home_prices.csv   # Raw dataset
│   ├── home_prices_model.pkl       # Trained model
│   ├── columns.json                # Location names & columns
├── static/                # CSS and assets
├── templates/             # HTML templates
├── requirements.txt       # Project dependencies
└── README.md              # Project documentation
```

---

## 💻 How to Run Locally

```bash
# Step 1: Clone the repository
git clone https://github.com/DikshithML/Real-Estate.git
cd Real-Estate

# Step 2: Create and activate virtual environment
python -m venv venv
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate

# Step 3: Install dependencies
pip install -r requirements.txt

# Step 4: Run the app
python app.py
```

🌐 Open in browser: `http://localhost:5000`

---

## 🧠 Model Details

- Trained using cleaned housing price data
- Input features: location, total sqft, BHK, number of bathrooms
- Outputs price in lakhs (₹)
- Model serialized with `joblib`
- Location list is dynamically populated from `columns.json`

---

## ⚠️ Notes

- Make sure `home_prices_model.pkl` and `columns.json` are inside the `model/` directory
- Extendable to other cities or with more features like amenities, property age, etc.
- You can integrate maps, charts, or user login system for advanced features

---

## 📜 License

This project is licensed under the **MIT License**.  
Feel free to fork, enhance, or deploy it freely.

---

> Made with ❤️ by Dikshith ML
