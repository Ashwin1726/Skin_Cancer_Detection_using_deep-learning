<div align="center">

🩺 Skin Cancer Detection

Deep Learning • Computer Vision • Flask

An image-based deep learning application for classifying skin lesions into seven diagnostic categories.

<br/>

<img src="model_architecture.png" width="720" alt="CNN Model Architecture"/>

<br/><br/>






</div>

✨ Overview

This project uses a Convolutional Neural Network (CNN) to analyze uploaded skin images and classify them into 7 lesion categories.

The trained model is integrated with a Flask web application, allowing a user to upload an image and receive the model's predicted class together with informational content.

⚠️ Research / educational project only. Predictions must not be treated as a medical diagnosis. Always consult a qualified dermatologist or healthcare professional.

🧠 Model

The project uses a custom CNN implemented with TensorFlow / Keras.

Input Image
    │
    ▼
28 × 28 × 3
    │
    ▼
Convolution + ReLU
    │
    ▼
Max Pooling + Batch Normalization
    │
    ▼
Convolution Blocks
    │
    ▼
Flatten + Dropout
    │
    ▼
Dense Layers
    │
    ▼
Softmax
    │
    ▼
7-Class Prediction

Architecture Highlights

Convolutional layers: 16 → 32 → 64 → 128 → 256 filters

ReLU activations

Max pooling

Batch normalization

Dropout regularization

Dense classification layers

Final 7-class Softmax output

Trained weights loaded from best_model.h5

🔬 Supported Classes

#

Classification

01

Actinic keratoses & intraepithelial carcinomae

02

Basal cell carcinoma

03

Benign keratosis-like lesions

04

Dermatofibroma

05

Melanocytic nevi

06

Pyogenic granulomas & hemorrhage

07

Melanoma

⚡ Application Flow

Upload Skin Image
        ↓
Image Resize
    28 × 28 × 3
        ↓
CNN Inference
        ↓
Softmax Probabilities
        ↓
Highest-Probability Class
        ↓
Result + Information

The Flask application exposes:

GET /          → Upload interface
POST /showresult → Image prediction

🖥️ Web Interface

The application provides:

📤 Skin-image upload

👁️ Image preview before submission

🧠 CNN-based prediction

📋 Result information

🔗 Project blog & code references

🛠️ Tech Stack

Language
Python

Machine Learning
TensorFlow Keras CNN NumPy

Computer Vision
OpenCV Pillow

Web
Flask HTML CSS Bootstrap

Development
Jupyter Notebook Google Colab

📁 Project Structure

Skin_Cancer_Detection_using_deep-learning/
│
└── skin/
    ├── app.py
    ├── skin_cancer_detection.py
    ├── best_model.h5
    ├── model_architecture.png
    ├── skin_project.ipynb
    │
    ├── templates/
    │   ├── summa.html
    │   └── reults.html
    │
    ├── static/
    │   ├── gif.gif
    │   └── gif2.gif
    │
    └── smaples/
        └── sample skin images

🚀 Run Locally

1. Clone

git clone https://github.com/YOUR_USERNAME/Skin_Cancer_Detection_using_deep-learning.git
cd Skin_Cancer_Detection_using_deep-learning/skin

2. Install dependencies

pip install tensorflow flask pillow numpy

3. Make sure the trained model exists

skin/
└── best_model.h5

4. Start Flask

python app.py

5. Open

http://127.0.0.1:5000

📌 Key Implementation

The application:

Receives an uploaded image through Flask.

Opens the image using Pillow.

Resizes it to 28 × 28.

Converts it into a NumPy array.

Passes the image into the trained CNN.

Selects the highest-probability class.

Displays the predicted category and related information.

📊 Project Assets

Asset

Purpose

best_model.h5

Trained CNN weights

model_architecture.png

Neural-network architecture

skin_project.ipynb

Project notebook

report.pdf

Project report

app.py

Flask application

templates/

Web interface

🔗 References

Project Blog
https://skincareaware.blogspot.com/2024/10/skin-cancer-detection-using-machine.html

Google Colab / Code
https://colab.research.google.com/drive/1kkP2r1Lhu3jPSLg-7nmU4SA8IBD5FN1w

<div align="center">

👨‍💻 Developed by Ashwin Kumar

AI/ML Engineer · Full-Stack Developer

<a href="https://www.linkedin.com/in/ashwin2617">
<img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>

<a href="mailto:ashwinkumaras59@gmail.com">
<img src="https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>

<br/><br/>

⭐ If you find this project useful, consider starring the repository.

</div>
