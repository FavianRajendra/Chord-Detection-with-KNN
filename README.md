🎸 Signal to Song: KNN Musical Chord Recognition

This repository contains a Jupyter Notebook (Chord Detections.ipynb) demonstrating a complete machine learning pipeline for classifying simple musical chords from synthetic time-series data.

The project uses Signal Processing techniques (like filtering and FFT) to extract meaningful features from raw sound waves and employs a K-Nearest Neighbors (KNN) classifier to perform the final chord recognition.

🌟 Project Overview

The goal of this project is to model and classify four fundamental musical chords: C Major, G Major, A Major, and E minor (Em). The approach is entirely data-driven, simulating the audio signal generation, extracting key features, and training a classification model.

Key Steps in the Pipeline:

Synthetic Data Generation: Creation of controlled time-series data mimicking the combined sine waves (harmonics) that define specific chord frequencies.

Signal Pre-processing: Application of digital filtering to clean the raw time-series signals.

Feature Engineering: Extraction of robust features in both the time domain and frequency domain (using FFT) to convert raw signal data into a format suitable for machine learning.

Classification: Training and evaluation of the K-Nearest Neighbors (KNN) algorithm.

🛠️ Technology Stack

Component

Technology

Role

Language

Python

Core programming language.

Classification

Scikit-learn (KNN)

Machine learning model used for chord classification.

Signal Processing

SciPy (scipy.signal, scipy.fft)

Used for filtering, Fast Fourier Transform, and entropy calculation.

Data Handling

NumPy, Pandas

Fundamental array and data manipulation.

Visualization

Matplotlib, Seaborn

Used for plotting raw signals, frequency spectrums, and evaluation plots (Pairplot, Confusion Matrix).

📐 Extracted Features

The model relies on a diverse set of engineered features, including:

Time Domain: Mean, Standard Deviation, Variance.

Frequency Domain: Dominant frequency components extracted via FFT.

Statistical/Information Theory: Signal entropy.

🚀 Getting Started

To run this notebook and reproduce the results, you will need a Python environment with the required packages.

Prerequisites

pip install numpy pandas scikit-learn matplotlib seaborn scipy jupyter


Execution

Clone the repository:

git clone [Your-Repo-URL]
cd [repository-name]


Start Jupyter Notebook:

jupyter notebook "Chord Detections.ipynb"


Run all cells sequentially to generate the data, extract features, train the KNN model, and view the performance evaluation.
