# 😀 Face Emotion Detection using Deep Learning (CNN)

A complete end-to-end deep learning project that detects human emotions from facial expressions in **real-time** using a Convolutional Neural Network (CNN) built with TensorFlow/Keras and OpenCV.

From raw dataset preprocessing to live webcam predictions — this repo covers the full pipeline.

---

## 📌 Features

- 🖼️ Preprocessing of facial emotion datasets (grayscale conversion + resizing)
- 🧠 Custom CNN architecture using `Conv2D`, `MaxPooling2D`, `Flatten`, and `Dense` layers
- 📊 Model training & validation with TensorFlow/Keras
- 📷 Real-time emotion detection via webcam using OpenCV
- 🧾 Fully commented, beginner-friendly code

---

## 🧠 Tech Stack

| Category | Tools |
|---|---|
| Language | Python |
| Deep Learning | TensorFlow, Keras |
| Computer Vision | OpenCV |
| Data Handling | NumPy, Pandas |
| Visualization | Matplotlib |

---

## 📁 Project Structure

```
face-emotion-detection/
│
├── original_dataset/                 # Training & validation images (per-emotion folders)
├── preprocessed_dataset/                 # Training & validation images (peprocessed folders)
├── Face_Emotion_Detector.ipynb        # Dataset loading & preprocessing
├── Model_Building.ipynb              # CNN model building & training
├── Model.keras              # Saved trained model
├── webcam.ipynb              # Real-time webcam emotion detection
└── README.md
```

---

## 📂 Dataset

This project uses a labeled facial emotion dataset organized into folders per emotion class (e.g., `Happy`, `Sad`, `Angry`, `Surprise`, `Neutral`, `Fear`, `Disgust`).

Download the dataset here: **[Project Files](https://www.kaggle.com/datasets/msambare/fer2013)**

Place the extracted dataset inside the `dataset/` directory before training.

---

## 🚀 Usage

### 1. Train the model
```bash
python src/Model_Building.ipynb
```

### 2. Run real-time detection
```bash
python src/webcam.ipynb
```
Press **`q`** to quit the webcam window.

---

## 🏗️ Model Architecture

```
Input (48x48 grayscale)
   → Conv2D + ReLU → MaxPooling2D
   → Conv2D + ReLU → MaxPooling2D
   → Conv2D + ReLU → MaxPooling2D
   → Flatten
   → Dense + Dropout
   → Dense (Softmax, num_classes)
```

---

## 📈 Results

| Metric | Value |
|---|---|
| Training Accuracy | 0.91 |
| Validation Accuracy | 0.89 |

---

## 🔍 Real-World Applications

- 🛡️ Smart surveillance & security systems
- 🛍️ Customer emotion analysis in retail
- 🤖 Emotion-aware chatbots & interactive AI
- 🧘 Mental health tracking tools
