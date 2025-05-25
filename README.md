
# ✈️ Flight Fare Prediction Web App

A machine learning-powered Flask web application that predicts flight ticket prices based on various travel parameters such as airline, source, destination, number of stops, and journey time.

---

## 🚀 Features

- Predicts flight fares using a Random Forest Regression model
- User-friendly web interface built with Flask & HTML
- Handles multiple airlines, routes, and date-time inputs
- Clean one-hot encoding and input preprocessing
- CORS-enabled for frontend integration

---

## 🧠 Tech Stack

- **Backend:** Python, Flask
- **ML Model:** Random Forest Regressor (trained using Scikit-Learn)
- **Frontend:** HTML5, CSS3 (Bootstrap optionally)
- **Libraries:** Pandas, Scikit-learn, Pickle, Flask-CORS

---

## 📁 Project Structure

```
├── app.py
├── models/
│   └── flight_rf.pkl
├── templates/
│   └── home.html
├── static/
│   └── style.css (optional)
└── README.md
```

---

## 🧑‍💻 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/flight-fare-predictor.git
cd flight-fare-predictor
```

### 2. Create a virtual environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the app

```bash
python app.py
```

Visit `http://127.0.0.1:5000` in your browser.

---

## 🧪 Sample Input Parameters

- Departure Time: `2023-07-24T12:45`
- Arrival Time: `2023-07-24T16:00`
- Airline: `Jet Airways`
- Source: `Delhi`
- Destination: `Cochin`
- Stops: `1`

---

## 📊 Model Training (Optional)

The model was trained on a cleaned dataset from Kaggle. If you wish to retrain:

```python
from sklearn.ensemble import RandomForestRegressor
model = RandomForestRegressor()
model.fit(X_train, y_train)
pickle.dump(model, open("models/flight_rf.pkl", "wb"))
```

---

## 🛡️ License

This project is licensed under the [MIT License](LICENSE).

---

## 🙌 Acknowledgments

- [Kaggle Flight Price Dataset](https://www.kaggle.com/datasets)
- [Flask Documentation](https://flask.palletsprojects.com/)
- [Scikit-learn Documentation](https://scikit-learn.org/)

---

## 📬 Contact

Created with ❤️ by [Deep Samanta](https://github.com/deep12112002)
