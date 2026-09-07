
# 🩺 Skin Cancer Detection

### Deep Learning • Computer Vision • Flask

<p>
  <b>AI-powered skin lesion classification using a custom CNN model</b>
</p>

<p>
  <img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/TensorFlow-ML-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/Keras-Deep%20Learning-D00000?style=for-the-badge&logo=keras&logoColor=white"/>
  <img src="https://img.shields.io/badge/Flask-Web%20App-000000?style=for-the-badge&logo=flask&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenCV-Computer%20Vision-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white"/>
</p>

<p>
  <a href="https://github.com/YOUR_USERNAME/Skin_Cancer_Detection_using_deep-learning">
    <img src="https://img.shields.io/badge/GitHub-Repository-181717?style=flat-square&logo=github"/>
  </a>
  <a href="https://skincareaware.blogspot.com/2024/10/skin-cancer-detection-using-machine.html">
    <img src="https://img.shields.io/badge/Project-Blog-FF5722?style=flat-square&logo=blogger&logoColor=white"/>
  </a>
</p>

</div>

---

## 🔬 Overview

**Skin Cancer Detection** is a deep learning-based computer vision project
that classifies skin lesion images into **7 different categories** using a
custom **Convolutional Neural Network (CNN)**.

The trained model is integrated with a **Flask web application**, allowing
users to upload an image and receive a predicted class through a simple
web interface.

> **Image → Preprocessing → CNN → Classification → Result**

---

## ✨ Features

| | Feature | Description |
|---|---|---|
| 🧠 | **Custom CNN** | Deep learning model for skin lesion classification |
| 🔬 | **7-Class Prediction** | Supports seven different lesion categories |
| 📷 | **Image Upload** | Upload skin images through the web interface |
| 👁️ | **Image Preview** | Preview the selected image before prediction |
| ⚡ | **Real-Time Inference** | Generate predictions through the Flask backend |
| 🌐 | **Web Interface** | Simple browser-based prediction system |
| 📊 | **Softmax Output** | Produces probability scores for each class |
| 📓 | **Jupyter Notebook** | Model experimentation and development |

---

## 🧬 Supported Classes

The model is configured to classify the following **7 categories**:

| # | Skin Lesion Category |
|:---:|---|
| 01 | Actinic Keratoses & Intraepithelial Carcinomae |
| 02 | Basal Cell Carcinoma |
| 03 | Benign Keratosis-like Lesions |
| 04 | Dermatofibroma |
| 05 | Melanocytic Nevi |
| 06 | Pyogenic Granulomas & Hemorrhage |
| 07 | Melanoma |

---

## 🏗️ Model Architecture

The project uses a custom **TensorFlow/Keras CNN** with convolution,
pooling, batch normalization, dropout and dense layers.

<div align="center">

<img src="skin/model_architecture.png" width="850"/>

</div>

### Architecture Flow

```text
                    INPUT
                 28 × 28 × 3
                      │
                      ▼
              ┌───────────────┐
              │ Conv2D (16)    │
              └───────┬───────┘
                      ▼
                Max Pooling
                      │
              Batch Normalization
                      │
                      ▼
              Conv2D (32 → 64)
                      │
                Max Pooling
                      │
              Batch Normalization
                      │
                      ▼
             Conv2D (128 → 256)
                      │
                      ▼
                   Flatten
                      │
                   Dropout
                      │
                Dense Layers
                      │
              Batch Normalization
                      │
                   Dropout
                      │
                      ▼
                  Softmax
                      │
                      ▼
                7-Class Output

```
---

# 🚀 Getting Started

Get the project running locally in just a few steps.

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/Skin_Cancer_Detection_using_deep-learning.git
cd Skin_Cancer_Detection_using_deep-learning

2️⃣ Enter the Application Directory
cd skin
3️⃣ Create a Virtual Environment

Windows

python -m venv venv
venv\Scripts\activate

macOS / Linux

python3 -m venv venv
source venv/bin/activate
4️⃣ Install Dependencies
pip install tensorflow flask pillow numpy
5️⃣ Verify the Trained Model

Make sure the trained model is available inside the skin directory:

skin/
└── best_model.h5

💡 The application uses best_model.h5 for image classification and prediction.

6️⃣ Run the Application
python app.py
7️⃣ Open in Browser

Once the Flask server starts, open:

<p align="center">

👉 http://127.0.0.1:5000

</p>
```

⚠️ Medical Disclaimer
<div align="center">
🩺 Educational & Research Purpose Only
</div>

This project is strictly intended for educational and research purposes.

The predictions generated by this application must not be considered
medical diagnoses and should not replace professional medical advice,
diagnosis, or treatment.

If you have any medical concern, please consult a qualified healthcare
professional.

.

🔗 Project Resources
<div align="center">
📚 Resource	🔗 Access
📖 Project Blog	Read the Blog
🧪 Google Colab	Open Notebook
</div>

<div align="center">
👨‍💻 Developed by Ashwin Kumar

AI/ML Engineer · Full-Stack Developer

<br> <a href="https://www.linkedin.com/in/ashwin2617/"> <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/> </a> <a href="mailto:ashwinkumaras59@gmail.com"> <img src="https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/> </a>

<br><br>

⭐ If you found this project interesting, consider starring the repository!

</div>


