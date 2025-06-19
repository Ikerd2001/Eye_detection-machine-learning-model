# Eye_detection-machine-learning-model

Purpose
The Eye Disease Detection System is an open-source web application designed to assist in the early identification of common eye diseases using deep learning and computer vision.
The system enables users to perform real-time eye disease analysis through their webcam or by uploading eye images.
This tool is intended for educational, research, and preliminary screening purposes, and is not a substitute for professional medical diagnosis.

Features
Real-time Webcam Analysis:
Instantly predicts eye diseases using your device’s camera.

Image Upload Analysis:
Upload an eye image for immediate AI-powered assessment.

Deep Learning Model:
Utilizes a pre-trained Keras/TensorFlow model for accurate multi-class classification.

User-Friendly Interface:
Simple navigation between live detection and image upload modes.

Technologies Used
Python 3.x

Flask (Web Framework)

TensorFlow / Keras (Deep Learning)

OpenCV (Computer Vision)

Pillow (Image Processing)

HTML/CSS (Jinja2 Templates)

Project Structure
text
eye-disease-detection/
│
├── app.py
├── model/
│   └── eye_disease_classifier.h5
├── static/
│   └── uploads/
├── templates/
│   ├── index.html
│   ├── video_feed.html
│   ├── upload.html
│   └── prediction.html
├── requirements.txt
└── README.md
Setup Instructions
1. Clone the Repository
bash
git clone https://github.com/your-username/eye-disease-detection.git
cd eye-disease-detection
2. Create a Virtual Environment (Recommended)
bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
3. Install Dependencies
bash
pip install -r requirements.txt
4. Place the Model
Download or train your Keras model (eye_disease_classifier.h5) and place it in the model/ directory.

5. Run the Application
bash
python app.py
6. Access the Web App
Open your browser and go to:
http://127.0.0.1:5000/

Usage
Live Camera Detection:
Click on "Real-time Camera Analysis" to start webcam-based predictions.

Image Upload:
Click on "Image Upload Analysis" to submit an eye image for analysis.

Results:
The system will display the predicted disease class and confidence score.
