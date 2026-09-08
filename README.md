<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:07111f,35:0ea5e9,65:14b8a6,100:061018&height=190&section=header&text=SKIN%20CANCER%20DETECTION&fontSize=38&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=DEEP%20LEARNING%20%7C%20COMPUTER%20VISION%20%7C%20FLASK&descAlignY=62&descSize=14" width="100%"/>

<h1>🧬 Skin Cancer Detection using Deep Learning</h1>

<p>
  <b>AI-powered skin lesion classification using a custom Convolutional Neural Network and a Flask web application.</b>
</p>

<br/>

<img src="https://img.shields.io/badge/DEEP%20LEARNING-CNN-0ea5e9?style=for-the-badge&logo=tensorflow&logoColor=white"/>
<img src="https://img.shields.io/badge/TENSORFLOW-KERAS-ff6f00?style=for-the-badge&logo=tensorflow&logoColor=white"/>
<img src="https://img.shields.io/badge/PYTHON-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/FLASK-WEB%20APP-000000?style=for-the-badge&logo=flask&logoColor=white"/>
<img src="https://img.shields.io/badge/COMPUTER%20VISION-ENABLED-14b8a6?style=for-the-badge"/>

<br/><br/>

<table>
<tr>
<td align="center" width="25%">
<h2>🧠</h2>
<b>CNN MODEL</b><br/>
7-Class Classification
</td>
<td align="center" width="25%">
<h2>🖼️</h2>
<b>IMAGE INPUT</b><br/>
28 × 28 × 3
</td>
<td align="center" width="25%">
<h2>⚡</h2>
<b>REAL-TIME</b><br/>
Flask Inference
</td>
<td align="center" width="25%">
<h2>🔬</h2>
<b>MEDICAL AI</b><br/>
Lesion Classification
</td>
</tr>
</table>

</div>

<div align="center">

🌟 PROJECT OVERVIEW

</div>

<p align="center">
This project uses a <b>TensorFlow/Keras Convolutional Neural Network (CNN)</b> to classify uploaded skin images into
<b>7 skin-lesion categories</b>. A Flask web application provides a simple interface where a user can upload an image,
the image is resized to <b>28 × 28</b>, passed through the trained model, and the predicted class with supporting information is displayed.
</p>

<div align="center">

<table>
<thead>
<tr>
<th>⚙️ COMPONENT</th>
<th>🔍 IMPLEMENTATION</th>
</tr>
</thead>
<tbody>
<tr>
<td><b>Model</b></td>
<td>TensorFlow / Keras Sequential CNN</td>
</tr>
<tr>
<td><b>Input</b></td>
<td>RGB image resized to 28 × 28 × 3</td>
</tr>
<tr>
<td><b>Output</b></td>
<td>7-class softmax prediction</td>
</tr>
<tr>
<td><b>Backend</b></td>
<td>Python + Flask</td>
</tr>
<tr>
<td><b>Image Processing</b></td>
<td>Pillow + NumPy</td>
</tr>
<tr>
<td><b>Model Weights</b></td>
<td><code>best_model.h5</code></td>
</tr>
</tbody>
</table>

</div>

<div align="center">

🧬 SUPPORTED CLASSES

</div>

<table>
<thead>
<tr>
<th>#</th>
<th>LESION CLASS</th>
<th>PROJECT LABEL</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center"><b>01</b></td>
<td>Actinic keratoses and intraepithelial carcinomae</td>
<td>🔴 Cancer</td>
</tr>
<tr>
<td align="center"><b>02</b></td>
<td>Basal cell carcinoma</td>
<td>🔴 Cancer</td>
</tr>
<tr>
<td align="center"><b>03</b></td>
<td>Benign keratosis-like lesions</td>
<td>🟢 Non-Cancerous</td>
</tr>
<tr>
<td align="center"><b>04</b></td>
<td>Dermatofibroma</td>
<td>🟢 Non-Cancerous</td>
</tr>
<tr>
<td align="center"><b>05</b></td>
<td>Melanocytic nevi</td>
<td>🟢 Non-Cancerous</td>
</tr>
<tr>
<td align="center"><b>06</b></td>
<td>Pyogenic granulomas and hemorrhage</td>
<td>🟠 Can Lead to Cancer</td>
</tr>
<tr>
<td align="center"><b>07</b></td>
<td>Melanoma</td>
<td>🔴 Cancer</td>
</tr>
</tbody>
</table>

<div align="center">

🧠 CNN ARCHITECTURE

</div>

<p align="center">
The project defines a <b>Sequential CNN</b> with convolutional layers, max-pooling, batch normalization,
dropout and dense layers before the final 7-class softmax output.
</p>

<div align="center">

<img src="./skin/model_architecture.png" alt="CNN Model Architecture" width="850"/>

</div>

<br/>

<table>
<thead>
<tr>
<th>LAYER</th>
<th>CONFIGURATION</th>
</tr>
</thead>
<tbody>
<tr><td>Input</td><td><code>28 × 28 × 3</code></td></tr>
<tr><td>Convolution</td><td>16 filters · 3 × 3 · ReLU · Same Padding</td></tr>
<tr><td>Pooling</td><td>MaxPool 2 × 2</td></tr>
<tr><td>Normalization</td><td>Batch Normalization</td></tr>
<tr><td>Convolution</td><td>32 filters · 3 × 3 · ReLU</td></tr>
<tr><td>Convolution</td><td>64 filters · 3 × 3 · ReLU</td></tr>
<tr><td>Pooling</td><td>MaxPool 2 × 2</td></tr>
<tr><td>Normalization</td><td>Batch Normalization</td></tr>
<tr><td>Convolution</td><td>128 filters · 3 × 3 · ReLU</td></tr>
<tr><td>Convolution</td><td>256 filters · 3 × 3 · ReLU</td></tr>
<tr><td>Flatten</td><td>Feature vector generation</td></tr>
<tr><td>Dropout</td><td>0.2</td></tr>
<tr><td>Dense</td><td>256 · ReLU</td></tr>
<tr><td>Dense</td><td>128 · ReLU</td></tr>
<tr><td>Dense</td><td>64 · ReLU</td></tr>
<tr><td>Dense</td><td>32 · ReLU</td></tr>
<tr><td>Output</td><td>7 units · Softmax</td></tr>
</tbody>
</table>

<div align="center">

🔄 PREDICTION PIPELINE

</div>

<table>
<tr>
<td align="center" width="16%"><h2>📤</h2><b>UPLOAD</b><br/>Skin Image</td>
<td align="center">➜</td>
<td align="center" width="16%"><h2>🖼️</h2><b>RESIZE</b><br/>28 × 28</td>
<td align="center">➜</td>
<td align="center" width="16%"><h2>🔢</h2><b>NUMPY</b><br/>RGB Tensor</td>
<td align="center">➜</td>
<td align="center" width="16%"><h2>🧠</h2><b>CNN</b><br/>Prediction</td>
<td align="center">➜</td>
<td align="center" width="16%"><h2>📊</h2><b>RESULT</b><br/>Class + Info</td>
</tr>
</table>

                    USER
                     │
                     ▼
              ┌─────────────┐
              │ Upload Image │
              └──────┬──────┘
                     │
                     ▼
              ┌─────────────┐
              │ Pillow      │
              │ Resize      │
              │ 28 × 28     │
              └──────┬──────┘
                     │
                     ▼
              ┌─────────────┐
              │ NumPy       │
              │ RGB Tensor  │
              └──────┬──────┘
                     │
                     ▼
          ┌─────────────────────┐
          │ TensorFlow / Keras  │
          │      CNN Model      │
          └──────────┬──────────┘
                     │
                     ▼
             ┌──────────────┐
             │ 7-Class      │
             │ Softmax      │
             └──────┬───────┘
                    │
                    ▼
             ┌──────────────┐
             │ Predicted    │
             │ Lesion Class │
             └──────────────┘

<div align="center">

💻 WEB APPLICATION

</div>

<p align="center">
The Flask interface contains an image upload workflow and a result page that displays the predicted class,
additional information associated with the class, and project resources.
</p>

<table>
<tr>
<td align="center" width="50%">
<h3>📤 INPUT PAGE</h3>
Upload a skin image<br/><br/>
<b>→ Preview image</b><br/>
<b>→ Submit for prediction</b>
</td>
<td align="center" width="50%">
<h3>📊 RESULT PAGE</h3>
Predicted lesion class<br/><br/>
<b>→ Class information</b><br/>
<b>→ Project resources</b>
</td>
</tr>
</table>

<div align="center">

🛠️ TECHNOLOGY STACK

</div>

<table>
<thead>
<tr>
<th>CATEGORY</th>
<th>TECHNOLOGY</th>
<th>ROLE</th>
</tr>
</thead>
<tbody>
<tr>
<td>🐍 Programming</td>
<td><b>Python</b></td>
<td>Application and ML development</td>
</tr>
<tr>
<td>🧠 Deep Learning</td>
<td><b>TensorFlow / Keras</b></td>
<td>CNN model architecture and inference</td>
</tr>
<tr>
<td>🖼️ Image Processing</td>
<td><b>Pillow</b></td>
<td>Image loading and resizing</td>
</tr>
<tr>
<td>🔢 Numerical Computing</td>
<td><b>NumPy</b></td>
<td>Image-to-array conversion</td>
</tr>
<tr>
<td>🌐 Backend</td>
<td><b>Flask</b></td>
<td>Web server and prediction routes</td>
</tr>
<tr>
<td>🎨 Frontend</td>
<td><b>HTML + CSS + Bootstrap</b></td>
<td>User interface and result presentation</td>
</tr>
<tr>
<td>📓 Experimentation</td>
<td><b>Jupyter / Google Colab Notebook</b></td>
<td>Project experimentation and development</td>
</tr>
</tbody>
</table>

<div align="center">

📁 PROJECT STRUCTURE

</div>

Skin_Cancer_Detection_using_deep-learning-main/
│
└── skin/
    │
    ├── app.py
    │   └── Flask application
    │
    ├── skin_cancer_detection.py
    │   └── CNN architecture + model loading
    │
    ├── best_model.h5
    │   └── Trained model weights
    │
    ├── skin_project.ipynb
    │   └── Project notebook
    │
    ├── model_architecture.png
    │   └── CNN architecture visualization
    │
    ├── wsgi.py
    │   └── WSGI entry point
    │
    ├── templates/
    │   ├── summa.html
    │   └── reults.html
    │
    └── smaples/
        └── Sample skin images

<div align="center">

⚙️ SETUP & INSTALLATION

</div>

01 — Clone the repository

git clone https://github.com/YOUR_USERNAME/Skin_Cancer_Detection_using_deep-learning.git
cd Skin_Cancer_Detection_using_deep-learning

02 — Enter the application folder

cd skin

03 — Create a virtual environment

<b>Windows</b>

python -m venv venv
venv\Scripts\activate

<b>macOS / Linux</b>

python3 -m venv venv
source venv/bin/activate

04 — Install dependencies

The current project imports Flask, Pillow, NumPy and TensorFlow/Keras:

pip install flask pillow numpy tensorflow

05 — Run the application

python app.py

The Flask application is configured to run on:

http://localhost:5000

Open the address in your browser and upload a skin image.

<div align="center">

🔌 APPLICATION ROUTES

</div>

<table>
<thead>
<tr>
<th>METHOD</th>
<th>ROUTE</th>
<th>FUNCTION</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>GET / POST</code></td>
<td><code>/</code></td>
<td>Displays the skin-image upload interface.</td>
</tr>
<tr>
<td><code>GET / POST</code></td>
<td><code>/showresult</code></td>
<td>Receives the uploaded image, performs CNN inference and displays the result.</td>
</tr>
</tbody>
</table>

<div align="center">

🧪 HOW PREDICTION WORKS

</div>

<p align="center">

<b>1.</b> User uploads an image
  →  
<b>2.</b> Flask receives the file
  →  
<b>3.</b> Pillow opens the image
  →  
<b>4.</b> Image is resized to <code>28 × 28</code>
  →  
<b>5.</b> NumPy converts it into the model input format
  →  
<b>6.</b> CNN predicts 7 class probabilities
  →  
<b>7.</b> Highest-probability class is selected
  →  
<b>8.</b> Result page displays the prediction and information

</p>

<div align="center">

📚 PROJECT RESOURCES

</div>

<table>
<tr>
<td align="center" width="50%">
<h3>📖 PROJECT BLOG</h3>
<a href="https://skincareaware.blogspot.com/2024/10/skin-cancer-detection-using-machine.html">
<b>Read the Complete Project Blog →</b>
</a>
</td>
<td align="center" width="50%">
<h3>🧪 GOOGLE COLAB</h3>
<a href="https://colab.research.google.com/drive/1kkP2r1Lhu3jPSLg-7nmU4SA8IBD5FN1w">
<b>Open Project Notebook →</b>
</a>
</td>
</tr>
</table>

<div align="center">

⚠️ MEDICAL DISCLAIMER

</div>

<table>
<tr>
<td align="center">⚠️</td>
<td>
<b>This project is for educational and research purposes only.</b>
<br/><br/>
The prediction generated by this application should <b>not</b> be considered a medical diagnosis.
Skin conditions can require professional examination and clinical testing. Users should consult a qualified
dermatologist or healthcare professional for medical evaluation and treatment decisions.
</td>
</tr>
</table>

<div align="center">

🚀 FUTURE ENHANCEMENTS

</div>

<table>
<tr>
<td>⬜</td><td>Improve image preprocessing and normalization</td>
<td>⬜</td><td>Model performance evaluation dashboard</td>
</tr>
<tr>
<td>⬜</td><td>Confidence score visualization</td>
<td>⬜</td><td>Grad-CAM explainable AI visualization</td>
</tr>
<tr>
<td>⬜</td><td>Modern responsive frontend</td>
<td>⬜</td><td>Cloud deployment</td>
</tr>
<tr>
<td>⬜</td><td>REST API documentation</td>
<td>⬜</td><td>Automated model monitoring</td>
</tr>
</table>

<div align="center">

👨‍💻 DEVELOPER

<h2>ASHWIN KUMAR</h2>

<p>
<b>AI/ML Engineer • Full-Stack Developer</b>
</p>

<p>
Interested in building practical AI systems using
<b>Deep Learning, Computer Vision and modern web technologies.</b>
</p>

<br/>

<a href="https://www.linkedin.com/in/ashwin1726/">
<img src="https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>

<br/><br/>

<a href="https://github.com/YOUR_USERNAME">
<img src="https://img.shields.io/badge/GITHUB-181717?style=for-the-badge&logo=github&logoColor=white"/>
</a>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:061018,35:14b8a6,65:0ea5e9,100:07111f&height=120&section=footer" width="100%"/>

<h3>🧬 SKIN CANCER DETECTION</h3>

<p><i>Deep Learning for Computer Vision</i></p>

⭐ <b>If you find this project useful, consider starring the repository!</b>

</div>
