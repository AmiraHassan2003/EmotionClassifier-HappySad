# HappySad Emotion Classifier 🎭

A lightweight CNN-based image classification model that detects facial emotions — **Happy** or **Sad** — using TensorFlow/Keras. Ideal for beginners and small-scale emotion recognition tasks.

---

## 📌 Project Overview

This project uses a simple Convolutional Neural Network (CNN) to classify facial expressions into two categories:

- 😊 Happy
- 😢 Sad

The dataset was collected from Google Images and organized into separate folders for each emotion. This project demonstrates fundamental deep learning steps including data preprocessing, model training, evaluation, and visualization.

---

## 🧠 Model Architecture

The model was built using TensorFlow's Sequential API:

```python
model.add(Conv2D(16, (3,3), 1, activation='relu', input_shape=(256,256,3)))
model.add(MaxPooling2D())

model.add(Conv2D(32, (3,3), 1, activation='relu'))
model.add(MaxPooling2D())

model.add(Conv2D(16, (3,3), 1, activation='relu'))
model.add(MaxPooling2D())

model.add(Flatten())
model.add(Dense(256, activation='relu'))
model.add(Dense(1, activation='sigmoid'))  # Binary classification
ذذذ
```

## 📊 Training Results

Precision: 1.0
Recall: 1.0
Accuracy: 1.0

### You can visualize training using TensorBoard:
     - tensorboard --logdir logs/


## 📈 Training Graphs

### Accuracy
   ![accuracy](https://github.com/user-attachments/assets/cea6b79a-470a-418d-b2f9-8d62b3ff4061)

### Loss
  ![loss](https://github.com/user-attachments/assets/840b6df7-b3fa-4efd-82a2-4bd1b18415a9)



## 📦 Requirements
  - Python 3.8+

  - TensorFlow 2.x

  - NumPy

  - Matplotlib

  - OpenCV (optional, for image handling)



## 🔮 Future Improvements
Add more emotion classes (angry, surprised, neutral)

Deploy model using Flask or Streamlit

Real-time webcam-based emotion detection

Improve dataset size and diversity

  
