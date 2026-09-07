<div align="center">

# 🩺 Skin Cancer Detection

### AI • Deep Learning • Computer Vision

**A CNN-powered web application for skin lesion classification using TensorFlow & Flask.**

<br/>

<img src="model_architecture.png" width="650" alt="CNN Model Architecture"/>

<br/><br/>

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)

<br/>

<a href="https://github.com/YOUR_USERNAME/Skin_Cancer_Detection_using_deep-learning">
<img src="https://img.shields.io/github/stars/YOUR_USERNAME/Skin_Cancer_Detection_using_deep-learning?style=social" />
</a>

</div>

---

## ✨ About The Project

**Skin Cancer Detection** is a Deep Learning and Computer Vision project
that uses a custom **Convolutional Neural Network (CNN)** to classify
uploaded skin images into **7 different lesion categories**.

The trained model is integrated into a **Flask web application**, allowing
users to upload an image and receive a model-generated classification result.

### 🎯 Objective

The goal of this project is to demonstrate how **Deep Learning + Computer
Vision + Web Development** can be combined to build an end-to-end image
classification application.

---

## 🧠 How It Works

```text
                📷
          Upload Skin Image
                 │
                 ▼
        ┌─────────────────┐
        │ Image Processing│
        │   28 × 28 × 3   │
        └────────┬────────┘
                 │
                 ▼
        ┌─────────────────┐
        │    CNN Model    │
        │ TensorFlow/Keras│
        └────────┬────────┘
                 │
                 ▼
        ┌─────────────────┐
        │  Classification │
        │   7 Classes     │
        └────────┬────────┘
                 │
                 ▼
             📊 Result
