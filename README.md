# DDoS Detection in IoT Networks Using CNN

This project is part of a collaborative research effort focused on detecting Distributed Denial of Service (DDoS) attacks in Internet of Things (IoT) environments. My primary contribution involved designing and implementing a lightweight convolutional neural network (CNN) to classify network traffic as benign or malicious based on extracted features.

## Abstract

The rapid proliferation of IoT devices has intensified the risk of Distributed Denial-of-Service (DDoS) attacks, underscoring the need for detection systems that are both accurate and lightweight enough for real-time deployment on resource-constrained hardware. This paper presents a two-stage DDoS detection framework designed specifically for IoT environments. In the first stage, we establish a baseline using Principal Component Analysis (PCA) for dimensionality reduction combined with a Multilayer Perceptron (MLP) classifier. In the second stage, a deep Autoencoder is used to extract compact feature representations, followed by lightweight classifiers including Logistic Regression, MLP, and a compact Convolutional Neural Network (CNN). The Autoencoder effectively reduces the feature set to five dimensions, significantly improving inference speed. Experimental results demonstrate that all Autoencoder-based models outperform the PCA-based baseline in efficiency. Notably, our lightweight MLP with five Autoencoder features achieves the best trade-off, with 98.88% accuracy and an inference time of just 6.25 μs per sample. These results highlight the potential of our method for real-time, resource-efficient DDoS detection in IoT systems

## My Contributions

- Developed a lightweight CNN architecture using PyTorch
- Trained and validated the model
- Measured inference time to assess real-time deployability
- Compared performance against an MLP baseline model

## Tools and Technologies

- Python, PyTorch
- Pandas, NumPy
- Matplotlib, Seaborn
- scikit-learn (for metrics and train/test split)

## Results

| Metric       | Score   |
|--------------|---------|
| Accuracy     | 99.86%  |
| F1 Score     | 0.9986  |
| AUC-ROC      | 0.9993  |
| Inference Time | 0.0101 ms |
