🧠 Breast Cancer Detection Using Pre-Processed Images and Ensemble Learning

This repository presents a machine learning approach to improve breast cancer detection using image pre-processing and classifier fusion techniques. The project implements and evaluates three classifiers—Convolutional Neural Network (CNN), K-Nearest Neighbors (KNN), and Decision Tree—on pre-processed mammogram images. It then fuses their results using ensemble methods to improve diagnostic accuracy.

📌 Abstract

Breast cancer is one of the leading causes of cancer-related deaths in women worldwide. While several machine learning techniques exist for its detection, their effectiveness is often limited by poor image quality. This work enhances detection accuracy by applying advanced image pre-processing techniques such as background removal, noise reduction, and contrast enhancement. The pre-processed images are classified using CNN, KNN, and Decision Tree models. The final diagnosis is improved through ensemble fusion techniques (mean and max), achieving superior performance over individual classifiers.

📊 Dataset

Name: CBIS-DDSM (Curated Breast Imaging Subset of DDSM)

Source: The Cancer Imaging Archive

Type: Mammography images (.jpg)

Total Images: ~10,239

Categories: Normal, Benign, Malignant

🔧 Methodology

1. Image Pre-processing
Noise Reduction: Median/Gaussian filtering

Contrast Enhancement: CLAHE

Normalization: Pixel intensity normalization

Segmentation: ROI and pectoral muscle separation

2. Classification Models
   
CNN: 4 convolution layers with filters 32, 64, 128, and 128; input size (50, 50, 3)

KNN: k=3, Euclidean distance metric

Decision Tree: Gini/Entropy-based splits

3. Fusion Techniques
   
Mean Fusion: Averaging classifier probabilities

Max Fusion: Taking maximum probability across classifiers

🧪 Results

Model	Accuracy
CNN	95%
KNN	90%
Decision Tree	85%
Fusion (Mean)	97%
Fusion (Max)	96%
