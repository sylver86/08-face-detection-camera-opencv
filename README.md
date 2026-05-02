# SmartLens — Rilevamento Facciale Real-Time con OpenCV

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-5C3EE8?logo=opencv&logoColor=white)
![Computer Vision](https://img.shields.io/badge/Computer%20Vision-Real--Time-green)
![Edge](https://img.shields.io/badge/Target-Embedded%20%2F%20Edge-orange)

## Panoramica

Sistema di rilevamento facciale real-time con OpenCV ottimizzato per fotocamere digitali consumer e dispositivi con risorse computazionali limitate. Utilizza classificatori Haar Cascade per rilevamento volti su stream video in tempo reale, con gestione efficiente dei frame per minimizzare latenza e consumo CPU.

Competenze applicabili in sistemi di accesso fisico intelligente, videosorveglianza perimetrale, edge computing IoT e qualsiasi pipeline di Computer Vision embedded.

## Valore Enterprise

| Settore / Azienda | Rilevanza |
|-------------------|-----------|
| Difesa & Aerospazio (Leonardo) | Riconoscimento facciale per sistemi di sicurezza fisica |
| Utilities & Infrastrutture (Enel, Terna) | Accesso controllato a impianti critici |
| IT Consulting (NTT Data, Accenture) | Computer Vision per soluzioni IoT e Smart Building |
| Engineering Informatica | Integrazione CV in applicazioni enterprise embedded |

## Caratteristiche Tecniche

| Feature | Implementazione |
|---------|----------------|
| Rilevamento volti | Haar Cascade Classifier (OpenCV) |
| Stream video | Acquisizione real-time da webcam/file video |
| Performance | Ottimizzazione frame processing per bassa latenza |
| Visualizzazione | Bounding box dinamici su ogni frame rilevato |
| Target hardware | Desktop, laptop, embedded (Raspberry Pi compatibile) |

## Pipeline Computer Vision

```
Stream video (webcam / file)
        │
        ▼
Acquisizione frame (cv2.VideoCapture)
        │
        ▼
Conversione grayscale
        │
        ▼
Haar Cascade detectMultiScale()
        │
        ▼
Disegno bounding box + annotazioni
        │
        ▼
Output video annotato
```

## Setup

```bash
git clone https://github.com/sylver86/08-face-detection-camera-opencv.git
cd 08-face-detection-camera-opencv
pip install -r requirements.txt
jupyter notebook "notebooks/Face Detection per Fotocamere Digitali.ipynb"
```

## Struttura Repository

```
08-face-detection-camera-opencv/
├── notebooks/
│   └── Face Detection per Fotocamere Digitali.ipynb
├── requirements.txt
└── README.md
```

## Stack Tecnologico

`Python 3.8+` · `OpenCV 4.x` · `NumPy` · `Haar Cascade` · `Real-Time Video Processing`

---

---

# SmartLens — Real-Time Face Detection with OpenCV 🇬🇧

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-5C3EE8?logo=opencv&logoColor=white)

## Overview

Real-time face detection system with OpenCV optimised for consumer digital cameras and computationally constrained devices. Uses Haar Cascade classifiers on live video streams, with efficient frame management to minimise latency and CPU usage.

Applicable to smart physical access control, perimeter surveillance, IoT edge computing, and any embedded Computer Vision pipeline.

## Technical Features

| Feature | Implementation |
|---------|---------------|
| Face detection | Haar Cascade Classifier (OpenCV) |
| Video stream | Real-time from webcam or video file |
| Performance | Frame processing optimised for low latency |
| Visualisation | Dynamic bounding boxes on each detected frame |
| Target hardware | Desktop, laptop, embedded (Raspberry Pi compatible) |

## CV Pipeline

```
Video stream  →  Frame capture  →  Grayscale conversion
    →  Haar Cascade detectMultiScale()  →  Bounding box overlay  →  Annotated output
```

## Setup

```bash
git clone https://github.com/sylver86/08-face-detection-camera-opencv.git
cd 08-face-detection-camera-opencv
pip install -r requirements.txt
jupyter notebook "notebooks/Face Detection per Fotocamere Digitali.ipynb"
```

## Technologies

`Python 3.8+` · `OpenCV 4.x` · `NumPy` · `Haar Cascade` · `Real-Time Video Processing`
