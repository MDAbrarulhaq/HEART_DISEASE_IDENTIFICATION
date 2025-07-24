
# Heart Disease Identification Using PCG Sound  
  

This project uses deep learning and digital signal processing to identify heart disease using **PCG (Phonocardiogram) sound recordings**. It serves as an innovative and low-cost alternative to traditional 2D echocardiography for early heart disease detection.

---

## 🫀 Project Overview

Heart sounds (PCG) provide vital clues about cardiovascular health. Using machine learning, this project classifies PCG signals as:
- **Normal** or  
- **Abnormal** (indicative of disease)

This can assist doctors in early diagnosis using just heart sound recordings — especially in resource-constrained environments.

---

## 📁 Project Structure

```

HEART\_DISEASE\_IDENTIFICATION/
├── code.ipynb              ← Jupyter Notebook with full ML pipeline
├── dataset/                ← Contains PCG audio files (WAV)
├── features.npy            ← Pre-processed Mel-spectrogram features
├── labels.npy              ← Corresponding labels (0: normal, 1: abnormal)
├── README.md               ← Project description (this file)
└── LICENSE                 ← MIT License

````

---

## 🧠 Technologies Used

- Python
- NumPy
- TensorFlow / Keras
- Librosa (audio processing)
- Matplotlib
- Jupyter Notebook

---

## 🔬 Methodology

### 🟡 1. Data Source  
- PhysioNet 2016 Challenge Dataset  
- PCG recordings collected from real patients

### 🔵 2. Feature Extraction  
- Extracted **Mel-Spectrograms** from .wav files using `librosa`  
- Stored in `features.npy` for fast training

### 🔴 3. Classification  
- Used a **Convolutional Neural Network (CNN)** model  
- Input: 2D Mel-spectrogram images  
- Output: Binary classification → Normal / Abnormal

---

## 📊 Model Performance

| Metric     | Value      |
|------------|------------|
| Accuracy   | **~85–90%** (approx.) |
| F1-Score   | **High** on validation set |
| Framework  | Keras CNN model |

---

## ▶️ How to Run

1. Clone the repository:
```bash
git clone https://github.com/MDAbrarulhaq/HEART_DISEASE_IDENTIFICATION.git
cd HEART_DISEASE_IDENTIFICATION
````

2. Open the notebook:

```bash
jupyter notebook code.ipynb
```

3. Run all cells to:

* Load PCG sound features
* Train or load the trained CNN model
* Predict heart condition (Normal / Abnormal)

---

## 📌 Application Use-Cases

* Mobile health diagnostics
* Cardiac screening in rural areas
* Early detection of congenital heart defects
* Health monitoring using digital stethoscopes

---

## 👨‍💻 Author

**Md Abrarul Haq**
B.Tech CSE – Mini Project
[GitHub Profile](https://github.com/MDAbrarulhaq)

---

## 📄 License

This project is licensed under the **MIT License**.
See `LICENSE` for more info.

---

## 🙏 Acknowledgements

* [PhysioNet 2016 Challenge Dataset](https://physionet.org/content/challenge-2016/)

* Google Colab for model training

````

