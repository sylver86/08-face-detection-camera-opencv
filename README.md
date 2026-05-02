# Face Detection for Digital Cameras — OpenCV + Scikit-learn

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-5C3EE8?logo=opencv&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML%20Pipeline-F7931E?logo=scikit-learn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-F37626?logo=jupyter&logoColor=white)

## Overview

Facial detection system designed to operate within the **computational constraints of consumer-grade digital cameras**.
The project focuses on selecting and building a lightweight ML model capable of accurately localising faces in images and returning bounding box coordinates — without requiring a GPU or high-end hardware.

The work involved systematic literature research to identify algorithms offering the best accuracy-to-compute trade-off, followed by full pipeline implementation using OpenCV and Scikit-learn.

---

## Results

| Metric | Value |
|--------|-------|
| Detection approach | Haar Cascade + ML classifier |
| Pipeline | Scikit-learn end-to-end |
| Bounding box output | (x, y, width, height) per face |
| Target hardware | Low-power embedded / consumer camera |
| Cross-validation | k-fold applied during model selection |

---

## Project Workflow

1. **Dataset research & selection** — identified a public facial recognition dataset with diverse demographics and precise bounding box annotations
2. **Data preparation** — image normalisation, bounding box annotation, augmentation for class balance
3. **Literature review** — evaluated lightweight detection models (Haar Cascade, HOG+SVM, MTCNN) by accuracy and compute cost
4. **Pipeline construction** — Scikit-learn pipeline integrating preprocessing, feature extraction, and model inference
5. **Cross-validation & tuning** — k-fold cross-validation to select and optimise the final model
6. **Prediction output** — model returns face coordinates as bounding boxes for each detected face in the input image

---

## Key Design Decisions

- **Lightweight model selection**: prioritised inference speed over peak accuracy to meet embedded hardware constraints
- **Scikit-learn pipeline**: all stages (preprocessing → feature extraction → inference) encapsulated in a single reproducible pipeline object
- **Bounding box regression**: model trained to output precise spatial coordinates rather than just a detection flag

---

## Setup

```bash
git clone https://github.com/sylver86/08-face-detection-camera-opencv.git
cd 08-face-detection-camera-opencv
pip install opencv-python scikit-learn pandas numpy jupyter
jupyter notebook
```

Open `Face Detection per Fotocamere Digitali.ipynb` and run all cells.

---

## Technologies

`Python` · `OpenCV 4.x` · `Scikit-learn` · `NumPy` · `Pandas` · `Jupyter`
