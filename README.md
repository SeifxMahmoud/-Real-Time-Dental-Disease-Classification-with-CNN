# 🦷 AI-Powered Dental Disease Classifier

## 📌 Overview
This project implements a convolutional neural network (CNN) to classify dental X-ray images into diagnostic categories such as Cavity, Gum Disease, and Healthy. The goal is to assist healthcare professionals in rapid screening and enable insurers to leverage image-based diagnostics in underwriting and claims automation. The final model achieves **94% classification accuracy** and includes visualization tools such as Grad-CAM and confusion matrices for explainability.

## 🎯 Business Context
In reinsurance and health insurance, diagnostic speed and accuracy directly affect risk assessment, claims verification, and pricing models. Automating diagnostics using AI tools offers operational scalability and allows insurers to spot trends in morbidity and dental health at population levels.

## 🔍 Problem Statement
Manual classification of X-ray images is resource-intensive and subject to variability. This project aims to:
- Reduce the diagnostic burden on dental professionals
- Enable image-based insights for insurers and reinsurers
- Ensure explainability and reproducibility of AI-assisted diagnoses

## 🧪 Methodology

### Data Pipeline
- **Data Source**: Publicly available dental X-ray image datasets (or synthetic samples)
- **Preprocessing**: Image resizing (224x224), grayscale normalization, augmentation (rotation, zoom)
- **Training**: CNN (3 convolutional layers), batch normalization, dropout regularization
- **Evaluation Metrics**: Accuracy, F1 Score, confusion matrix, precision, recall

### Tools & Libraries
- Python, TensorFlow, Keras
- Matplotlib, Seaborn
- Scikit-learn for evaluation metrics
- PIL for visualization output

## 📈 Results
- **Test Accuracy**: 94%
- **Macro F1 Score**: 0.92
- **Grad-CAM Visualizations** confirmed model attention on disease-relevant features

## 💼 Insurance & Reinsurance Relevance
- **Underwriting**: Automate evaluation of dental diagnostics to assess health risk
- **Claims**: Validate diagnosis-driven claims with image-based evidence
- **Epidemiology**: Track regional trends in oral health using aggregate model outputs

## 🔁 Model Workflow Summary
1. **Data Collection**: Acquire and clean X-ray datasets  
2. **Preprocessing**: Resize, normalize, and augment images  
3. **Model Training**: Train CNN on preprocessed data  
4. **Evaluation**: Analyze confusion matrix and classification metrics  
5. **Deployment**: Export model for use in Flask-based APIs  

## 🧾 Requirements

```txt
tensorflow
keras
numpy
matplotlib
seaborn
scikit-learn
opencv-python
pillow
