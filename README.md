````markdown
# Classroom Facial Expression Recognition 📚🎭

This repository presents a deep learning-based system to monitor and analyze teachers' facial expressions in real-time classroom environments using Convolutional Neural Networks (CNN) and Recurrent Neural Networks (RNN).

## 🔍 Overview
The project detects five primary emotions — **Happy, Sad, Angry, Confused, Neutral** — from classroom video footage. It aims to:
- Enhance classroom engagement analysis.
- Improve transparency and teacher accountability.
- Support better education quality monitoring in under-resourced schools.

## 🧠 Techniques Used
- **CNN (ResNet-50)** for spatial feature extraction (facial landmarks like mouth, eyes, brows).
- **RNN (LSTM)** for temporal modeling of emotional transitions across frames.
- **Custom dataset** collected from real classrooms with manual frame-level labeling.
- **Preprocessing**: Frame extraction, resizing to 224×224, normalization.

## 🗂️ Dataset
- **Training**: Publicly available facial expression datasets.
- **Testing**: Real-world classroom videos recorded in natural lighting and teaching conditions.
- Labeled manually into 5 emotion categories.

## 🛠️ Features
- Real-time emotion prediction from video.
- Pipeline: Video → Frames → CNN (ResNet50) → Features → RNN (LSTM) → Emotion Class.
- Model evaluation through Accuracy, Precision, Recall, and F1-score.
- Visualizations via confusion matrices and emotion prediction examples.

## 📊 Results
| Metric     | CNN (ResNet50) | RNN (LSTM) |
|------------|----------------|------------|
| Accuracy   | 0.26           | 0.32       |
| Precision  | 0.26           | 0.26       |
| Recall     | 0.26           | 0.32       |
| F1-Score   | 0.20           | 0.25       |

> 🧪 **Observation**: RNN outperforms CNN in recognizing temporal emotional cues, especially for dynamic expressions like anger or surprise.

## 🔮 Future Work

* Add attention mechanisms to focus on expressive facial regions.
* Deploy on edge devices for on-site school monitoring.
* Improve performance on the neutral class using balanced datasets and augmentation.

