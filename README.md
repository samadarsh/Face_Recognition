# 🧑‍🔬 Face Recognition using Machine Learning

A simple machine learning project to classify facial images of three individuals using image preprocessing and Logistic Regression.

---

## 📌 Overview

This project implements a basic face recognition pipeline:
- **Preprocessing** — Grayscale conversion and resizing to 640×640.
- **Feature Engineering** — Flattened pixel values (409,600 features).
- **Model** — Logistic Regression classifier.
- **Dataset** — Images of Jaden Smith, Maluma, and Mike Tyson.

---

## 🏗️ Project Structure

```
Face_Recognition/
├── dataset/
│   ├── jaden smith/
│   ├── maluma/
│   └── mike tyson/
├── Face_Recognition.ipynb  # Core pipeline & analysis
└── README.md
```

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** `scikit-image`, `scikit-learn`, `NumPy`, `Pandas`, `Matplotlib`
- **Environment:** Jupyter Notebook

---

## 📊 Quick Results

| Metric | Details |
|---|---|
| **Classes** | Jaden Smith, Maluma, Mike Tyson |
| **Input Size** | 640 × 640 (grayscale) |
| **Algorithm** | Logistic Regression |
| **Accuracy** | ~60% (Baseline) |

---

## 🔮 Future Scope

- [ ] Implement face detection (MTCNN/MediaPipe).
- [ ] Use PCA for dimensionality reduction.
- [ ] Experiment with CNNs or pre-trained embeddings (FaceNet).
- [ ] Refactor code for portability (relative paths).

