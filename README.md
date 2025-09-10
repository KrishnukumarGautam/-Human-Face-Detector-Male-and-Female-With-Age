👨👩 Gender & Age Detection
![Python](https://img.shields.io/badge/Python-3.10-blue)  
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)  
![OpenCV](https://img.shields.io/badge/OpenCV-Face%20Detection-green)  
![Gradio](https://img.shields.io/badge/Gradio-Web%20Interface-purple)  
![License](https://img.shields.io/badge/License-MIT-brightgreen)

A deep learning-based web application that detects human faces in an image and predicts their gender and age.
Built using TensorFlow, Keras, OpenCV, and Gradio, this project provides a real-time interface for face analysis.-

🌟 Features
✅ Detects multiple faces in an image
✅ Predicts gender (Male/Female) and age for each detected face
✅ Displays bounding boxes & labels
✅ Real-time web-based interface using Gradio
✅ Efficient multi-output CNN with MobileNetV2 backbone
✅ Custom data generator for age + gender labels

📁 Dataset
📌 UTKFace Dataset (~20,000 face images)
Labels: age, gender, ethnicity
Pre-aligned & cropped images
Must be downloaded manually from Kaggle or UTKFace repository

🛠 Tech Stack
Python 🐍
TensorFlow / Keras
OpenCV (Haarcascade for face detection)
Gradio (Web interface)
NumPy, Pandas
Matplotlib

🧠 Model Architecture
Backbone: MobileNetV2 (ImageNet weights, frozen)
Two Heads:
Gender → Binary classification (sigmoid)
Age → Regression (linear)

Training:
Loss → binary_crossentropy (gender), mse (age)
Optimizer → Adam
Metrics → accuracy (gender), mae (age)
Custom Data Generator: Batches images with labels for both gender & age

🚀 How to Run
# Clone repository
git clone https://github.com/KrishnukumarGautam/gender-age-detection.git
cd gender-age-detection
# Install dependencies
pip install -r requirements.txt
# Run notebook in Colab or locally
# Upload UTKFace dataset ZIP when prompted
# Train (or load pre-trained model)
# Launch Gradio app
python app.py

📊 Results
Train/Val/Test Split → 80/10/10
Test Gender Accuracy → ~83%
Test Age MAE → ~8.3 years
Training Curves

📈 Gender Accuracy vs Val Accuracy
📉 Gender Loss vs Val Loss
📊 Age MAE vs Val MAE
📉 Age Loss (MSE) vs Val Loss


🔮 Future Work
🚀 Improve with data augmentation
📸 Add real-time webcam detection
🌍 Add ethnicity prediction from UTKFace
📱 Optimize for mobile deployment

🤝 Contribution
Contributions are welcome!
1. Fork the repo 🍴
2. Create a branch 🌿
3. Commit changes ✅
4. Open a Pull Request 🚀

📄 License

MIT License © 2025 Krishnu Kumar Gautam


---

👨‍💻 Author
Krishnu Kumar Gautam
B.Tech CSE (AI & Data Science), 5th Semester
AKS University, Satna
