

# 🩸 Blood Group Classification System (Fingerprint-Based)

## 📘 Overview

The **Blood Group Classification System** is a machine learning application that predicts an individual's **blood group type** using **fingerprint images**.
It combines **image processing** and **deep learning** to classify fingerprints into corresponding blood group categories and provide their **biological names**.

This project demonstrates the potential of biometrics in healthcare diagnostics, identification systems, and emergency response support.

---

## 🚀 Features

* 🖐️ Accepts **fingerprint images** as input
* 🔍 Predicts **blood group type** (`A+`, `A−`, `B+`, `B−`, `AB+`, `AB−`, `O+`, `O−`)
* 🧬 Displays **biological name** (e.g., *Type A positive*, *Type O negative*)
* 📊 Provides **prediction confidence score**
* 🧠 Uses a **Convolutional Neural Network (CNN)** trained on preprocessed fingerprint datasets
* 🌐 Ready for integration with a **Flask web interface** or **API service**

---

## 🧩 System Architecture

1. **Data Input:** Fingerprint image uploaded by the user
2. **Preprocessing:** Image resizing, noise reduction, and feature extraction
3. **Model Prediction:** CNN model predicts the most probable blood group class
4. **Result Display:** Shows predicted class, confidence, and biological name

---

## 🧠 Model Details

* **Architecture:** Custom CNN (or transfer learning using `InceptionV3` / `ResNet50`)
* **Input Shape:** 224x224 or 128x128 grayscale images
* **Output Classes:** 8 (A+, A−, B+, B−, AB+, AB−, O+, O−)
* **Frameworks:** TensorFlow / Keras
* **Optimizer:** Adam
* **Loss Function:** Categorical Crossentropy
* **Activation Function:** Softmax

---

## 🖥️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/blood-group-system.git
cd blood-group-system
```

### 2️⃣ Create a Virtual Environment

```bash
python -m venv venv
venv\Scripts\activate   # (Windows)
source venv/bin/activate  # (Linux/Mac)
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Application

```bash
python app.py
```

Then open your browser and navigate to `http://127.0.0.1:5000/`

---

## 🧪 Example Output

**Input:** Fingerprint image
**Output:**

```
Predicted Class: B+
Biological Name: Type B positive
Confidence: 94.2%
```


---

## 🧬 Biological Names Reference

| Class | Biological Name  |
| ----- | ---------------- |
| A+    | Type A positive  |
| A−    | Type A negative  |
| B+    | Type B positive  |
| B−    | Type B negative  |
| AB+   | Type AB positive |
| AB−   | Type AB negative |
| O+    | Type O positive  |
| O−    | Type O negative  |

---

## 📊 Future Enhancements

* Integration with **fingerprint sensors (e.g., R305, DigitalPersona)**
* Support for **real-time classification** via webcam or sensor feed
* **Explainable AI (XAI)** visualizations (e.g., Grad-CAM) to show fingerprint regions influencing classification
* Integration with hospital or donor databases

---

## 🧑‍💻 Author

**Julius Babatunde**
ML & AI Developer | Biometrics & Predictive Systems

---

Would you like me to make it **Flask-ready**, meaning I include short sections for how it interacts with the model and displays predictions on a web interface (so you can use it directly for your MVP)?
