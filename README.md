Markdown

# 🎶 Signal to Song: KNN Musical Chord Recognition

This repository contains a machine learning project that demonstrates a full pipeline for classifying common musical chords from synthetic audio signals.

The project combines **signal processing** techniques (filtering, FFT) to extract features and uses the **K-Nearest Neighbors (KNN)** algorithm for classification.

## 🌟 Project Highlights

* **Custom Data Generation:** Generates synthetic time-series data for four common chords (C, G, A, Em) by simulating their harmonic structure.
* **Feature Engineering Pipeline:** Converts complex raw signal data into a robust feature set using time-domain statistics and **Fast Fourier Transform (FFT)** for frequency analysis.
* **Classification:** Implements and evaluates a **K-Nearest Neighbors (KNN)** model for chord recognition.
* **Evaluation:** Visualizes model performance using classification metrics and a **Confusion Matrix**.

## 🛠️ Technology Stack

| Component | Technology | Role |
| :--- | :--- | :--- |
| **Language** | Python | Core development language. |
| **Classification** | **Scikit-learn (KNN)** | Machine learning algorithm for final classification. |
| **Signal Processing** | **SciPy** (`scipy.signal`, `scipy.fft`) | Used for filtering and frequency domain analysis. |
| **Data Handling** | NumPy, Pandas | Array and tabular data manipulation. |
| **Visualization** | Matplotlib, Seaborn | Plotting signals, spectrums, and evaluation metrics. |

---

## 📂 Data & Methodology

### 1. Target Chords
The model is trained to classify the following four chords:
* **C Major**
* **G Major**
* **A Major**
* **E minor (Em)**

### 2. Feature Extraction
The feature set used for training the KNN model includes, but is not limited to:
* **Time Domain:** Mean, Standard Deviation, and Variance of the signal.
* **Frequency Domain:** Dominant frequency components (using FFT).
* **Signal Statistics:** Signal Entropy.

The notebook carefully visualizes the raw signals and their FFT spectrums to ensure features are meaningful representations of the underlying audio data.

---

## 🚀 Getting Started

Follow these steps to set up the project and run the analysis locally.

### Prerequisites

Ensure you have Python installed. Then, install all necessary libraries using pip:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn scipy jupyter
Execution
Clone the repository:

Bash

git clone [https://github.com/FavianRajendra/TF-IDF-and-Cosine-Similarity.git](https://github.com/FavianRajendra/TF-IDF-and-Cosine-Similarity.git)
cd TF-IDF-and-Cosine-Similarity
Run the Notebook: Open the Jupyter Notebook in your environment.

Bash

jupyter notebook "Chord Detections.ipynb"
Execute all cells in the notebook sequentially to generate the data, extract features, train the model, and view the final classification results.

📝 Project Summary
This project showcases an end-to-end data science application in audio analysis. By creating controlled signal data and applying appropriate digital signal processing techniques, we successfully transform raw audio concepts into trainable data for a simple yet effective machine learning model, achieving reliable chord classification.
