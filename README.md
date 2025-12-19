# EEG-Based-Emotion-Recognition-using-Deep-Neural-Networks
Decoding Emotional Valence through Computational Neuroscience

# Project Overview
This study implements a robust machine learning pipeline for the automated classification of emotional states (Negative, Neutral, Positive) using EEG (Electroencephalogram) signal data. The project bridges the gap between raw neurophysiological data and computational modeling, achieving high-fidelity classification of neural signals.

The primary objective is to demonstrate the efficacy of Deep Learning (Sequential MLP) in identifying acute emotional markers, providing a scalable framework for research in emotional regulation and stress response.

# Dataset and Methodology
The analysis is based on a structured dataset of EEG features acquired via Muse headband technology.

Signal Sources: TP9, AF7, AF8, TP10 electrode positions.

Feature Engineering: The dataset incorporates statistical descriptors (mean, standard deviation) and spectral power components derived from Fast Fourier Transform (FFT) analysis.

Target Classes: Tri-class classification (Negative, Neutral, Positive valence).

# Experimental Results
Final Test Accuracy: 99.06%

Model Convergence: The learning curves (Accuracy/Loss Dynamics) demonstrate stable convergence with a minimal generalization gap, indicating high robustness on unseen data.

Classification Performance: The confusion matrix indicates a high degree of separability between all classes, with particularly distinct clusters for negative emotional states.

# Neuroscientific Feature Analysis
To move beyond "black-box" prediction, a Feature Importance Analysis was conducted to identify the critical biomarkers of emotional valence:

Primary Predictor: min_q_10_b was identified as the most significant feature, reflecting the role of signal minima in emotional state differentiation.

Spectral Significance: FFT-derived features emerged as dominant predictors, confirming that frequency-domain shifts (associated with Beta and Gamma band power) are essential indicators of emotional arousal.

Cortical Dominance: Features originating from the AF7 and AF8 sensors (Prefrontal Cortex) exhibited high predictive weight, aligning with established neurobiological theories regarding the PFC's role in emotional regulation and valence processing.

Statistical Distribution
A box plot analysis of the top features confirms a clear statistical separation across emotional categories. The distinct distribution of min_q_10_b across states provides a validated biological basis for the model's high performance.

# Technical Specifications
Framework: TensorFlow / Keras

Implementation: Python

Key Libraries: Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib

Architecture: Multi-Layer Perceptron (MLP) with Batch Normalization and Dropout layers for optimized regularization.

# Conclusion and Future Work
This project validates the use of deep learning for real-time neuro-classification. Future iterations could integrate these models into longitudinal studies, such as the Police-In-Action (PIA) research, to predict behavioral outcomes like "freezing" or "avoidance" under acute stress.

Zeynep Şirin 
