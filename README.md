🛡️ PhishX – Browser Extension for Phishing Alerts

PhishX is a **browser-based phishing detection system** implemented as a Chrome Extension that uses **Machine Learning** to identify and alert users about potentially harmful websites in real-time.
The project focuses on improving web security by analyzing URLs and webpage content to prevent phishing attacks.

---

🚀 Features

* 🔍 **Real-time phishing detection** while browsing
* 🧠 **Machine Learning model (XGBoost)** for high accuracy predictions
* 📊 Extracts **30+ URL and webpage features** for analysis
* ⚡ **FastAPI backend** for fast and efficient predictions
* 🔗 Seamless **REST API integration** between extension and backend
* 📦 Lightweight and easy-to-use Chrome extension
* 🔐 **Privacy-friendly** – no personal user data is stored
* 🚨 Instant **visual alerts (Safe / Phishing warning)**

---

🧩 Project Structure

```
PhishX/
│
├── frontend/        # Chrome Extension (HTML, CSS, JS)
│
├── backend/         # FastAPI backend + ML model
│   ├── app.py
│   ├── url_feature_extractor.py
│   └── best_xgb_model.pkl
│
├── dataset/         # Dataset used for training
│
├── notebook/        # ML training & evaluation
│
└── README.md
```

---

🛠️ Technologies Used

**Machine Learning:**

* XGBoost
* Scikit-learn

**Frontend:**

* HTML
* CSS
* JavaScript
* Chrome Extension APIs

**Backend:**

* Python
* FastAPI

**Tools & Libraries:**

* Pandas
* NumPy
* Joblib
* BeautifulSoup

---

⚙️ How It Works

1. User visits a website 🌐
2. Extension captures the **URL and page data**
3. Features are extracted using custom logic
4. Data is sent to the **FastAPI backend**
5. ML model predicts whether the site is **Safe or Phishing**
6. User receives an **instant alert on the screen**

---

🧪 Setup & Installation

1️⃣ Clone the Repository

```
git clone https://github.com/Meghana-07-ops/PhishX_Detector_Extension.git
cd PhishX_Detector_Extension
```

2️⃣ Install Backend Dependencies

```
pip install -r requirements.txt
```

*(or install manually if requirements.txt is not available)*

3️⃣ Run Backend Server

```
uvicorn app:app --reload
```

---

4️⃣ Load Chrome Extension

1. Open Chrome → `chrome://extensions/`
2. Enable **Developer Mode**
3. Click **Load Unpacked**
4. Select the `frontend/` folder

---

📊 Output

* ✅ Safe websites → Green indicator
* ⚠️ Phishing websites → Warning popup
* 🔄 Same domain → Smart detection (avoids repeated scanning)

---

🎯 Project Objective

The goal of this project is to provide a **simple, effective, and real-time solution** for detecting phishing attacks and improving user awareness while browsing the internet.

---

👥 Team Contribution

* Backend & ML Model
* Chrome Extension Development
* UI/UX Design
* Testing & Debugging
* Documentation

---

🔮 Future Improvements

* 📈 Display **risk percentage** instead of binary result
* 🧠 Improve model accuracy with larger dataset
* 🗂️ Add **scan history dashboard**
* 🌐 Support for **email phishing detection**
* 🔐 Integration with **real-time threat intelligence APIs**

---

📜 License

This project is developed for educational purposes and follows an open-source approach.

---

