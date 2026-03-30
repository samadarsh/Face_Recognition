# 🧑‍🔬 Face Recognition System

A machine learning-based face recognition system that classifies facial images into three categories using image preprocessing and supervised learning techniques.

---

## 📌 Overview

This project implements an end-to-end face recognition pipeline using classical computer vision and machine learning. The system processes facial images through grayscale conversion, resizing, and pixel-level feature extraction, then trains a Logistic Regression classifier to distinguish between three individuals.

### Key Highlights
- **Image Preprocessing** — Automated resizing, grayscale conversion, and normalization using `scikit-image`
- **Feature Engineering** — Flattened pixel representation creating a high-dimensional feature space (409,600 features)
- **Classification** — Supervised learning with Logistic Regression achieving baseline accuracy on the test set
- **Visualization** — Confusion matrix and prediction analysis using `matplotlib`

---

## 🏗️ Architecture

```
Face_Recognition/
├── dataset/
│   ├── jaden smith/      # 50 face images
│   ├── maluma/           # 52 face images
│   └── mike tyson/       # 51 face images
├── Face_Recognition.ipynb  # Main notebook (end-to-end pipeline)
└── README.md
```

### Pipeline Flow

```
Raw Images (RGB) ──→ Resize (640×640) ──→ Grayscale Conversion
       │
       ▼
Flatten to 1D Vector (409,600 features) ──→ DataFrame Assembly
       │
       ▼
Train/Test Split ──→ Logistic Regression ──→ Prediction & Evaluation
```

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| Language | Python 3.x |
| Image Processing | scikit-image (`skimage`) |
| Data Handling | NumPy, Pandas |
| ML Model | scikit-learn (Logistic Regression) |
| Visualization | Matplotlib |
| Environment | Jupyter Notebook |

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8 or higher
- pip (Python package manager)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/samadarsh/Face_Recognition.git
   cd Face_Recognition
   ```

2. **Install dependencies**
   ```bash
   pip install numpy pandas matplotlib scikit-image scikit-learn
   ```

3. **Launch the notebook**
   ```bash
   jupyter notebook Face_Recognition.ipynb
   ```

4. **Update dataset paths** — Modify the file paths in the notebook to point to the local `dataset/` directory.

---

## 📊 Results

| Metric | Value |
|---|---|
| Classes | 3 (Jaden Smith, Maluma, Mike Tyson) |
| Training Samples | ~120 |
| Test Samples | ~30 |
| Image Dimensions | 640 × 640 (grayscale) |
| Feature Vector Size | 409,600 |
| Model | Logistic Regression |
| Accuracy | ~60% |

---

## 🔮 Future Improvements

- [ ] **Face Detection & Cropping** — Integrate MTCNN or MediaPipe to isolate face regions before classification
- [ ] **Dimensionality Reduction** — Apply PCA to reduce the 409K feature space to a manageable dimension
- [ ] **Advanced Models** — Experiment with SVM (RBF kernel), Random Forest, or lightweight CNNs
- [ ] **Deep Embeddings** — Use pre-trained FaceNet/ArcFace models for 128D face embeddings (target: 90%+ accuracy)
- [ ] **Data Augmentation** — Apply rotations, flips, and brightness adjustments to expand the training set
- [ ] **Code Refactoring** — Modularize image loading and preprocessing into reusable utility functions
- [ ] **Relative Paths** — Replace hardcoded absolute paths with portable relative paths

---

## 📧 Contact

**Adarsh S** — [GitHub](https://github.com/samadarsh)

---

## 📄 License

This project is open source and available for educational purposes.
