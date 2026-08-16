# Automated Solar Panel Fault Detection Using Hybrid Wavelet Transform and Deep Learning

> Undergraduate thesis project — B.Sc. in Electrical & Electronic Engineering, Khulna University of Engineering & Technology (KUET)

![Status](https://img.shields.io/badge/status-completed-success)
![Field](https://img.shields.io/badge/domain-Renewable%20Energy-blue)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-TensorFlow%2FKeras-orange)

### 📄 [**Read the Full Thesis Report (PDF)**](../../raw/main/Overleaf_Upload__2_.pdf)

---

## 📖 Overview

Solar photovoltaic (PV) panels degrade and develop faults over time — from shading and soiling to cell cracks and hotspots. Undetected faults reduce energy yield and can pose safety risks. Manual inspection of large solar installations is slow and expensive.

This project presents an **automated fault-detection framework** that combines **hybrid wavelet-transform-based feature extraction** with a **deep learning classifier** to detect and categorize solar-panel faults automatically, enabling faster and more reliable maintenance of renewable-energy systems.

---

## 🎯 Objectives

- Extract meaningful fault signatures from PV signal/image data using wavelet transforms.
- Train a deep neural network to classify healthy vs. faulty panels (and fault types).
- Improve detection accuracy and reliability compared to conventional threshold-based methods.
- Contribute toward efficient, low-cost, automated monitoring of solar installations.

---

## 🧠 Approach

```
   PV Data
      │
      ▼
┌──────────────────────┐
│  Pre-processing      │   Cleaning, normalization
└──────────────────────┘
      │
      ▼
┌──────────────────────┐
│  Hybrid Wavelet      │   Multi-level feature extraction
│  Transform           │   (captures fault signatures)
└──────────────────────┘
      │
      ▼
┌──────────────────────┐
│  Deep Learning       │   Neural network classifier
│  Network             │   (fault detection & classification)
└──────────────────────┘
      │
      ▼
   Fault / No-Fault  +  Fault Type
```

---

## 🗂️ Repository Structure

```
├── src/         # Source code (feature extraction, model, training, evaluation)
├── data/        # Dataset info and sample data (see data/README.md)
├── models/      # Saved/trained model files
├── results/     # Plots, confusion matrices, performance metrics
├── docs/        # Thesis report, presentation, figures
└── README.md    # This file
```

---

## 🛠️ Tech Stack

- **Language:** Python
- **Deep Learning:** TensorFlow / Keras
- **Signal Processing:** Wavelet transform (PyWavelets)
- **Data / Plotting:** NumPy, Pandas, Matplotlib, scikit-learn

---

## 📊 Results

The proposed **hybrid wavelet + weighted dual-backbone deep learning model** was evaluated against baseline methods for solar-panel fault classification. Key findings:

- The weighted dual-backbone architecture outperformed the standalone EfficientNet baseline.
- Strong classification performance across all fault categories, confirmed by the confusion matrices below.
- Demonstrated reliable automated detection suitable for real-world PV monitoring.

> _Add your headline metric here, e.g.:_ **Final model accuracy: __%**

### Performance Across All Methods
![Performance across all methods](results/IMG-20260803-WA0020.jpg)

### EfficientNet vs. Weighted Dual-Backbone
![EfficientNet vs Weighted Dual Backbone](results/IMG-20260803-WA0019.jpg)

### Final Confusion Matrix (Proposed Model)
![Final Confusion Matrix](results/IMG-20260803-WA0024.jpg)

### Binary Confusion Matrix
![Binary Confusion Matrix](results/IMG-20260803-WA0017.jpg)



## 🚀 How to Use

```bash
# Clone the repository
git clone https://github.com/DeadBat1727/solar-fault-detection.git
cd solar-fault-detection

# Install dependencies
pip install -r requirements.txt

# Run training
python src/train.py

# Run evaluation
python src/evaluate.py
```

---

## 📄 Thesis Report

The full thesis report is available here: **[Overleaf_Upload__2_.pdf](../../raw/main/Overleaf_Upload__2_.pdf)**

---

## 👤 Author

**Mohammad Tanzid Ahmed**
B.Sc. in Electrical & Electronic Engineering, KUET
📧 tanzidvai39@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/tanzid-ahmed-517666343)

---

## 📝 License

This project is released under the [MIT License](LICENSE).
