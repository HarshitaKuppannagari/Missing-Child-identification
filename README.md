# 👁️ Missing Child Identification System

This project is a Django-based web application designed to help identify and locate missing children by comparing uploaded photos against a trained dataset using facial recognition and image processing techniques.

---

## 🚀 Features

- 🔐 **Login System**: Secure login for officials
- 📤 **Image Upload**: Upload images of found or missing children
- 🧠 **Facial Recognition**: Compares uploaded images with the dataset
- 🖼️ **Image Preview**: View uploaded images and their matches
- 📊 **Dataset Matching**: Displays potential matches from test images
- 📁 **Structured Folders**: Organized static files, templates, and models

---

## 🛠️ Technologies Used

- **Backend**: Django (Python)
- **Frontend**: HTML, CSS (with `templatemo_style.css`)
- **Image Processing**: OpenCV, Haar Cascades
- **Machine Learning**: Keras (for model training and matching)
- **Data Storage**: `.npy` files for feature arrays

---

## 📂 Folder Structure

MissingChilds/
│
├── MissingChild/ # Main Django settings and URLs
├── MissingChildApp/ # App logic: views, models, templates
│ ├── static/ # CSS, images, uploads
│ ├── templates/ # HTML pages
│ └── photo/ # Sample photos for comparison
├── model/ # Pretrained ML model files
├── testImages/ # Images to be tested
├── haarcascade_frontalface_default.xml
├── manage.py
└── run.bat

---

## 📷 Model Details

The model is trained using facial images and is stored in:
- `model/model_weights.h5`: Trained Keras model weights
- `model/model.json`: Model architecture
- `model/X.txt.npy`, `Y.txt.npy`: Features and labels
- `model/history.pckl`: Training history

---

### 📈 Future Improvements

✅ Severity score for prediction match

📱 Mobile responsive interface

🌍 Geo-tagging found child reports

📄 PDF Report Generation (for authorities)

🔒 Multi-user roles (Admin, Police, NGO)
