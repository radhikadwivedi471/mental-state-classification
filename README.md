# EEG-Frequency-Band-Analysis

## **Project Overview**
This project focuses on **mental state classification using EEG signals**. The goal is to classify EEG segments as either **relaxed** or **focused** using machine learning techniques. The approach involves:

- Extracting **frequency-based features** (Alpha and Beta power, Alpha/Beta ratio) from EEG signals.
- Computing **statistical features** (mean, variance) from each EEG channel.
- Using these features to train a **Support Vector Machine (SVM)** classifier.
- Visualizing EEG signals, feature distributions, and model performance.

## **Dataset**
We use the **MNE sample dataset**:
- File: `sample_audvis_raw.fif`
- Channels: EEG only
- Epoch length: 2 seconds

## **Libraries Used**
- `mne` : EEG signal processing
- `numpy` : Numerical operations
- `scikit-learn` : Machine learning (SVM)
- `matplotlib` & `seaborn` : Visualization

## **Code Overview**
1. Load EEG data using MNE.
2. Filter EEG signals between **1–40 Hz**.
3. Create **fixed-length epochs** (2 seconds).
4. Extract **features per epoch**:
   - Alpha power (8–12 Hz)
   - Beta power (13–30 Hz)
   - Alpha/Beta ratio
   - Mean & Variance per channel
5. Train an **SVM classifier** to classify relaxed vs focused states.
6. Evaluate model performance with **accuracy** and **confusion matrix**.
7. Visualize EEG signals, features, and results.

## **Model Performance**
- **Accuracy:** ~`your_accuracy_here`
- Confusion matrix visualizes true vs predicted labels.

## **Important Plot**
 **EEG Signal Plot**  
   Example: First channel of first epoch


