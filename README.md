# EEG-Based Machine Learning for Dystonia Subtype Classification

This repository contains all the code and data processing steps used in the study:  
**"Decoding Dystonia: unveiling neural patterns with interpretable EEG-Based Machine Learning"**  
by Caroline L. Alves et al.

## 📌 Project Overview

This work proposes a novel and interpretable machine learning framework using EEG data to distinguish between:
- **Upper Limb Dystonia (ULD)**
- **Cervical Dystonia (CD)**
- **Healthy Controls (HC)**

We apply both traditional machine learning (ML) and deep learning (DL) approaches, combining:
- Complex network features
- Classical EEG signal metrics
- SHAP interpretability
- Task comparisons (resting, handwriting, finger tapping)

---

## 🧠 Repository Structure

- `EEG-measures-final.ipynb`: Computes traditional EEG metrics (e.g., bandpower).
- `Calculate-all--complex-network-measures-final.ipynb`: Extracts complex network features from connectivity matrices.
- `Export-matrices-final.ipynb`: Prepares and exports correlation/TE-based connectivity matrices from EEG.
- `Machine-Learning-parallelized-final.ipynb`: Runs classical ML models (SVM, RF, NB, etc.) with hyperparameter tuning.
- `CNN-tunning-final.ipynb`: Trains and tunes a CNN model to classify subjects based on EEG-derived matrices.
- `LSTM-final.ipynb`: LSTM architecture for EEG sequence modeling.
- `measures.py`: Helper functions for network and signal processing.

---

## 🛠️ Installation

To reproduce the results, clone this repository and set up a Python environment using:

```bash
git clone https://github.com/Carol180619/Paper-dystonia.git
cd Paper-dystonia
python -m venv venv
source venv/bin/activate  # On Windows use venv\Scripts\activate
pip install -r requirements.txt

## 🚀 How to Use

1. **Preprocess EEG Data**  
   Use `Export-matrices-final.ipynb` to filter EEG into frequency bands and build connectivity matrices.

2. **Feature Extraction**  
   Use `EEG-measures-final.ipynb` and `Calculate-all--complex-network-measures-final.ipynb` to extract both classical EEG features and complex network features.

3. **Train ML Models**  
   Use `Machine-Learning-parallelized-final.ipynb` to train and evaluate traditional machine learning classifiers (e.g., SVM, Random Forest, Naive Bayes).

4. **Train Deep Models**  
   Use `CNN-tunning-final.ipynb` or `LSTM-final.ipynb` to train and evaluate deep learning models on EEG-derived connectivity matrices.

---

## 📬 Contact

For questions or collaborations, please contact:  
**Caroline L. Alves**  
📧 caroline.lourenco.alves@gmail.com

