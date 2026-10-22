# Face Emotion Detection

An end-to-end computer-vision and deep-learning project for classifying facial expressions from images and webcam frames.

## Pipeline

1. Prepare and preprocess labeled facial-expression images.
2. Train a CNN with TensorFlow/Keras.
3. Save the trained model as `Model.keras`.
4. Run webcam inference with OpenCV.

## Repository map

- `Face_Emotion_Detector.ipynb` — loading and preprocessing
- `Model_Building.ipynb` — CNN training
- `webcam.ipynb` — real-time inference
- `Model.keras` — saved model artifact
- `original_dataset/` and `preprocessed_dataset/` — project data directories

## Setup

```bash
pip install tensorflow keras opencv-python numpy pandas matplotlib jupyter
jupyter notebook
```

Run the notebooks in the order shown above. Keep the dataset paths aligned with the local checkout.

## Limitations

Emotion classification is an approximation and can be affected by lighting, pose, dataset bias, and camera quality. It should not be used to make sensitive decisions about people.
