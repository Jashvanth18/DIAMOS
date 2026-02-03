# DiaMOS Pear Leaf Disease & Severity Classification

## Overview
This project implements a **dual-track deep learning framework** for automated **pear leaf disease classification and severity assessment** using the **DiaMOS dataset**, collected under real-field conditions.

---

## Objectives
- Classify pear leaf diseases accurately  
- Predict **five levels of disease severity (0–4)**  
- Handle real-world variations in lighting, background, and infection patterns  

---

## Dataset
- **Dataset:** DiaMOS Plant Dataset  
- **Classes:** Healthy, Leaf Curl, Leaf Spot, Pear Slug  
- **Severity Levels:** 0 (No Risk) to 4 (High Severity)  
- **Images:** RGB field images captured using smartphones and DSLR cameras  

---

## Methodology

### Track 1 – CNN-Based Feature Learning
- EfficientNet-B0 (pretrained)
- Group Shuffle Depthwise Convolution (GSDW)

### Track 2 – Graph-Based Context Modeling
- Graph Convolutional Network (GCN)
- Nodal Attention
- Coordinate Attention
- Global Context Network

### Feature Fusion
- Features from both tracks are fused
- Global Average Pooling + Fully Connected Layer for final prediction

---

## Results
- **Overall Accuracy:** **98.87%**
- High performance across all disease classes and severity levels
- Strong generalization on real-field data
- Grad-CAM visualizations confirm focus on disease regions

---

## Tech Stack
- Python
- PyTorch, PyTorch Geometric
- OpenCV, NumPy, Matplotlib
- NVIDIA T4 GPU (AWS EC2)
- Optimizer: Adam
- Mixed Precision Training (AMP)

---

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- Specificity

---

## Future Work
- Extend to other crops and diseases
- Deploy as a web/mobile application
- Add temporal disease progression analysis

---

## Author
**Jashvanth K**  
B.Tech CSE (AI & ML)  
SRM Institute of Science and Technology

