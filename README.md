DiaMOS Pear Leaf Disease & Severity Classification
📌 Project Overview

This project focuses on automated pear leaf disease detection and severity assessment using the DiaMOS dataset, captured under real-field conditions. A dual-track deep learning framework is proposed to jointly classify multiple pear leaf diseases and estimate their corresponding severity levels with high accuracy.

🎯 Objectives

Detect and classify pear leaf diseases accurately

Predict five levels of disease severity from leaf images

Handle real-world variations in lighting, background, and infection patterns

Improve interpretability and robustness using attention mechanisms

🗂 Dataset

Dataset: DiaMOS Plant Dataset

Leaf Classes: Healthy, Leaf Curl, Leaf Spot, Pear Slug

Severity Levels: 0 (No Risk) to 4 (High Severity)

Images: Real-field RGB images captured using smartphones and DSLR cameras

Annotations: Expert-labeled disease and severity ground truth

🧠 Methodology
🔹 Track 1: CNN-Based Feature Extraction

EfficientNet-B0 (pretrained) for global feature learning

Group Shuffle Depthwise Convolution (GSDW) to enhance channel interaction with low computational cost

🔹 Track 2: Graph-Based Context Modeling

Graph Convolutional Network (GCN) for relational feature learning

Nodal Attention to prioritize important graph nodes

Coordinate Attention for spatial and channel awareness

Global Context Network to capture long-range dependencies

🔹 Feature Fusion

Outputs from both tracks are fused and passed through Global Average Pooling and a Fully Connected Layer for final prediction.

📊 Results

Disease Classification Accuracy: 98.87%

High performance across all disease classes and severity levels

Strong generalization on real-field images

Grad-CAM visualizations confirm focus on disease-affected regions

🛠 Tech Stack

Programming Language: Python

Frameworks: PyTorch, PyTorch Geometric

Libraries: NumPy, OpenCV, Matplotlib

Hardware: NVIDIA T4 GPU (AWS EC2)

Optimizer: Adam

Training: Mixed Precision (AMP), Grid Search Hyperparameter Tuning

📈 Evaluation Metrics

Accuracy

Precision

Recall

F1-Score

Specificity

🔍 Visualization

Grad-CAM heatmaps used for model interpretability

Highlights lesion areas and severity regions on pear leaves

🚀 Future Work

Extend to other fruit crops and diseases

Deploy as a web or mobile application for farmers

Integrate temporal analysis for disease progression monitoring

👤 Author

Jashvanth K
B.Tech CSE (AI & ML)
SRM Institute of Science and Technology
