# 🩺 Disease Prediction System

### 🔬 Django Web App Powered by Machine Learning

![Repo
Banner](https://via.placeholder.com/1200x300?text=Disease+Prediction+System)

A smart medical assistance tool that predicts diseases based on symptoms
using machine learning.

------------------------------------------------------------------------

## 🏷️ Badges

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)\
![Django](https://img.shields.io/badge/Django-5.2-green.svg)\
![Machine Learning](https://img.shields.io/badge/ML-Powered-orange.svg)\
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)\
![Status](https://img.shields.io/badge/Status-Active-success.svg)

------------------------------------------------------------------------

## 📖 About the Project

The **Disease Prediction System** is a Django web app powered by a
machine learning model.\
Users select symptoms, and the model predicts the most likely disease.\
Each prediction is stored as **medical history** using Django ORM.

------------------------------------------------------------------------

## 🌟 Features

-   🩺 AI-powered predictions\
-   🧠 Trained ML model (`best_model.pkl`)\
-   📊 Saves prediction history\
-   🎨 Clean & responsive UI\
-   🛡️ Secure Django backend

------------------------------------------------------------------------

## 🧱 Project Architecture

    Frontend (HTML/CSS/Bootstrap)
            ↓
    Django Views & URL Routing
            ↓
    ML Model (best_model.pkl)
            ↓
    Prediction + Label Encoding
            ↓
    SQLite Database (History)

------------------------------------------------------------------------

## 🧪 Tech Stack

  Category         Tools
  ---------------- ------------------------------
  **Backend**      Django, Python
  **Frontend**     HTML, CSS, Bootstrap
  **ML**           Scikit-Learn, Pandas, Joblib
  **Database**     SQLite
  **Deployment**   WSGI/ASGI

------------------------------------------------------------------------

## 📷 Screenshots

### 🏠 Home Page

*(snapshot image provided by user)*

### 🩺 Prediction Page

*(snapshot image provided by user)*

### 📜 Medical History

*(snapshot image provided by user)*

------------------------------------------------------------------------

# ⚙️ Installation & Running the Project

## **1️⃣ Clone the Repository**

``` bash
git clone https://github.com/your-username/disease-prediction-system.git
cd disease-prediction-system
```

## **2️⃣ Create a Virtual Environment**

``` bash
python -m venv venv
```

### **Activate the Environment**

#### Windows:

``` bash
venv\Scriptsctivate
```

#### macOS / Linux:

``` bash
source venv/bin/activate
```

------------------------------------------------------------------------

## **3️⃣ Install Dependencies**

If you have a `requirements.txt`:

``` bash
pip install -r requirements.txt
```

If not, typical dependencies include:

``` bash
pip install django pandas scikit-learn joblib
```

------------------------------------------------------------------------

## **4️⃣ Apply Database Migrations**

``` bash
python manage.py migrate
```

------------------------------------------------------------------------

## **5️⃣ Run the Development Server**

``` bash
python manage.py runserver
```

Navigate to:\
👉 http://127.0.0.1:8000/

------------------------------------------------------------------------

## 🧠 How Prediction Works

1.  User selects symptoms (Yes=1, No=0)\
2.  Data is converted into a Pandas DataFrame\
3.  `best_model.pkl` predicts a disease class\
4.  `label_encoder.pkl` converts it into disease name\
5.  Prediction is saved into `History`\
6.  Result returned to user

------------------------------------------------------------------------

## 🗄 Database Model

    History
     ├── fever
     ├── headache
     ├── nausea
     ├── vomiting
     ├── fatigue
     ├── joint_pain
     ├── skin_rash
     ├── cough
     ├── weight_loss
     ├── yellow_eyes
     └── res (Predicted disease)

------------------------------------------------------------------------

## 📂 Project Structure

    myproject/
    │── myproject/
    │   ├── settings.py
    │   ├── urls.py
    │   ├── wsgi.py
    │   └── asgi.py
    │
    │── myapp/
    │   ├── models.py
    │   ├── views.py
    │   ├── admin.py
    │   ├── templates/
    │   │   ├── index.html
    │   │   ├── prediction.html
    │   │   └── history.html
    │   ├── best_model.pkl
    │   ├── label_encoder.pkl
    │
    ├── db.sqlite3
    ├── manage.py
    └── README.md

------------------------------------------------------------------------

## 🚀 Deployment Guide (Render / Railway / PythonAnywhere)

### **1. Push code to GitHub**

### **2. Install dependencies automatically**

### **3. Set environment variables:**

    DEBUG=False
    SECRET_KEY=your-secret-key

### **4. Run migrations**

### **5. Upload pickle files to the server**

### **6. Deploy with Gunicorn/WSGI**

------------------------------------------------------------------------

## 🤝 Contributing

1.  Fork the repo\
2.  Create a feature branch\
3.  Commit & push your changes\
4.  Submit a Pull Request

------------------------------------------------------------------------

## 📄 License

This project is licensed under the **MIT License**.

------------------------------------------------------------------------

## 👨‍💻 Developer

**Inzamamul Haq Siddiqui**
