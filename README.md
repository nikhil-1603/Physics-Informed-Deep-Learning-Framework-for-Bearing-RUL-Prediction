# Physics-Informed Deep Learning Framework for Bearing RUL Prediction

A novel deep learning framework for Remaining Useful Life (RUL) prediction of rolling element bearings using Physics-Informed Health Indicator (HI) learning, Multi-Scale Multi-Head Attention (MSMHA), and Autoencoder-based latent degradation representation.

---

# Overview

This repository presents a Physics-Informed Deep Learning architecture designed for accurate and stable bearing degradation assessment and Remaining Useful Life (RUL) prediction.

The framework integrates:

- Multi-Scale Multi-Head Attention (MSMHA)
- Autoencoder-based unsupervised feature learning
- Physics-informed Health Indicator optimization
- Monotonic degradation regularization
- Deep RUL regression learning

The proposed method learns degradation-sensitive latent representations directly from vibration signals and improves:

- Prediction accuracy
- HI monotonicity
- Temporal consistency
- Robustness against noise
- Long-term degradation tracking

---

# Key Features

✅ Physics-informed Health Indicator learning  
✅ Multi-Scale Multi-Head Attention (MSMHA)  
✅ Autoencoder-based latent feature extraction  
✅ End-to-end deep RUL prediction  
✅ Monotonic degradation optimization  
✅ Smooth degradation trajectory learning  
✅ Noise-robust representation learning  
✅ PyTorch implementation  
✅ Predictive maintenance framework  

---

# Proposed Framework

## Overall Pipeline

```text
Raw Vibration Signal
        ↓
Signal Preprocessing
        ↓
Multi-Scale Feature Extraction
        ↓
MSMHA Encoder
        ↓
Latent Degradation Representation
        ↓
Physics-Informed HI Optimization
        ↓
RUL Prediction Network
        ↓
Remaining Useful Life Estimation
```

---

# Methodology

## 1. Signal Processing

Raw bearing vibration signals are segmented and normalized before feature extraction.

---

## 2. Autoencoder-Based Representation Learning

A deep Autoencoder is used to learn compact degradation-sensitive latent representations from high-dimensional vibration data.

Advantages:
- Noise reduction
- Compact feature embedding
- Unsupervised degradation learning

---

## 3. Multi-Scale Multi-Head Attention (MSMHA)

The MSMHA module captures:

- Local degradation characteristics
- Global temporal dependencies
- Frequency-aware failure signatures
- Multi-scale degradation patterns

This improves degradation feature extraction from complex bearing signals.

---

## 4. Physics-Informed Health Indicator Learning

The latent Health Indicator (HI) is optimized using physics-guided degradation constraints:

### Constraints Used

- Monotonicity
- Trendability
- Smoothness
- Failure progression consistency

These constraints ensure physically meaningful degradation trajectories.

---

## 5. Remaining Useful Life Prediction

The optimized latent degradation representation is passed through a regression network to estimate Remaining Useful Life.

---

# Repository Structure

```text
├── data/
│   ├── train/
│   ├── test/
│
├── notebooks/
│   ├── MSMHA_AE_Physic_HI.ipynb
│
├── models/
│   ├── autoencoder.py
│   ├── msmha.py
│   ├── rul_predictor.py
│
├── utils/
│   ├── preprocessing.py
│   ├── metrics.py
│   ├── visualization.py
│
├── results/
│   ├── plots/
│   ├── checkpoints/
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

# Installation

## Clone the Repository

```bash
git clone https://github.com/your-username/physics-informed-rul-prediction.git
cd physics-informed-rul-prediction
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Requirements

```text
Python >= 3.9
PyTorch
NumPy
Pandas
SciPy
Scikit-learn
Matplotlib
Optuna
Jupyter Notebook
```

---

# Dataset

The framework can be evaluated on the following datasets:

- IEEE PHM Bearing Dataset
- XJTU-SY Bearing Dataset
- IMS Bearing Dataset
- FEMTO Bearing Dataset
- C-MAPSS (adaptable)

Place datasets inside the `data/` directory.

---

# Training

## Run Notebook

```bash
jupyter notebook notebooks/MSMHA_AE_Physic_HI.ipynb
```

---

## Train Using Python Script

```bash
python train.py
```

---

# Evaluation Metrics

The framework is evaluated using:

- RMSE
- MAE
- Score Function
- Monotonicity Index
- Trendability
- Prognosability
- Health Indicator Stability

---

# Experimental Advantages

The proposed framework provides:

- Better degradation representation
- Physically interpretable Health Indicators
- Stable long-term prediction
- Improved robustness against sensor noise
- Accurate end-of-life estimation
- Smooth degradation trajectory learning
- Better temporal consistency

---

# Example Results

## Health Indicator Trend

- Smooth monotonic degradation curve
- Stable degradation tracking
- Reduced fluctuation compared to conventional approaches

---

## RUL Prediction

- Accurate Remaining Useful Life estimation
- Lower prediction variance
- Improved temporal consistency

---

# Research Contributions

This work introduces:

1. Physics-guided latent Health Indicator learning
2. MSMHA-based degradation feature extraction
3. Joint unsupervised and supervised optimization
4. Monotonic degradation-aware learning
5. Stable degradation trajectory optimization

---

# Future Work

Potential future extensions include:

- Transformer-based degradation modeling
- Domain adaptation across datasets
- Self-supervised predictive maintenance
- Federated learning for industrial AI
- Edge-AI deployment for real-time monitoring
- Explainable AI for prognostics

---

# Applications

This framework can be applied to:

- Predictive Maintenance
- Bearing Fault Prognostics
- Industrial Condition Monitoring
- Smart Manufacturing
- Industry 4.0 Systems
- Rotating Machinery Health Monitoring

