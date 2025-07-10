# Diabetes Prediction System

This project is a web-based Diabetes Prediction System built using Django. It allows users to input medical information and predicts the likelihood of diabetes using a machine learning model (Logistic Regression) trained on the Pima Indians Diabetes Dataset.

## Features
- User-friendly web interface
- Predicts diabetes outcome based on user input
- Utilizes Logistic Regression for prediction
- Results displayed instantly on the web page

## Project Structure
```
djangoProject/
│   README.md
│   manage.py
│   db.sqlite3
│
├───DiabetesPrediction/
│   ├───DiabetesPrediction/
│   │   ├── asgi.py
│   │   ├── settings.py
│   │   ├── urls.py
│   │   ├── views.py
│   │   ├── wsgi.py
│   │   └── ...
│   ├───static/
│   ├───templates/
│   │    ├── home.html
│   │    └── predict.html
│   └───db.sqlite3
│
├───.venv/
└───.idea/
```

## How It Works
1. The user navigates to the home page and clicks "Let's get started".
2. The user fills out a form with medical details (Pregnancies, Glucose, Blood Pressure, Skin Thickness, Insulin, BMI, Diabetes Pedigree, Age).
3. The system uses a Logistic Regression model to predict whether the user is likely to have diabetes based on the input.
4. The result (Positive/Negative) is displayed to the user.

## Setup Instructions
1. **Clone the repository** and navigate to the project directory:
   ```bash
   git clone <repo-url>
   cd djangoProject
   ```
2. **Create a virtual environment** (recommended):
   ```bash
   python -m venv .venv
   .venv\Scripts\activate  # On Windows
   ```
3. **Install dependencies**:
   ```bash
   pip install django pandas scikit-learn matplotlib seaborn
   ```
4. **Ensure the dataset** (`diabetes.csv`) is placed at `C:/Users/new/OneDrive/Desktop/diabetes.csv` or update the path in `views.py`.
5. **Run migrations**:
   ```bash
   python manage.py migrate
   ```
6. **Start the development server**:
   ```bash
   python manage.py runserver
   ```
7. **Open your browser** and go to `http://127.0.0.1:8000/` to use the app.

## Dependencies
- Django
- pandas
- scikit-learn
- matplotlib
- seaborn

## Notes
- The machine learning model is trained each time a prediction is made (for demonstration purposes). For production, consider training and saving the model separately.
- The dataset used is the Pima Indians Diabetes Database. Make sure you have the CSV file available at the specified path.

## Author
- [Your Name Here]

---
*Generated on 2025-07-10*
