# PCB Fault Detection using U-Net

This project focuses on **detecting faults in Printed Circuit Boards (PCBs)** using a combination of 
**deep learning (U-Net segmentation)** and **classical image processing (adaptive thresholding)**.  
The goal is to automatically highlight PCB defects such as **burn marks, scratches, and missing 
components**.

---

## 🔍 Workflow

1. **Data Collection**
   - Images of real PCBs (both defect-free and faulty).
   - Preprocessed with resizing, normalization, and augmentation.

2. **Preprocessing**
   - Applied **adaptive thresholding** to enhance defect regions.
   - Converted RGB images to grayscale for defect localization.

3. **Model**
   - Implemented **U-Net** architecture for pixel-level segmentation.
   - Trained to generate binary masks highlighting faulty regions.

4. **Evaluation**
   - Accuracy / Dice Coefficient used to evaluate segmentation quality.
   - Qualitative evaluation with overlay of predicted masks.

5. **Results**
   - Successfully detected defects such as:
     - Burn marks
     - Scratches
     - Missing solder

---


## ⚙️ Tech Stack
- **Deep Learning**: U-Net (TensorFlow / PyTorch)
- **Image Processing**: OpenCV (Adaptive Thresholding)
- **Tools**: Python, NumPy, Matplotlib, Jupyter

---

## 🚀 Future Work
- Deploy trained model as a **web demo (Flask/Streamlit)**.
- Expand dataset with synthetic defect generation.
- Optimize training with transfer learning.

---

## 📌 Note
This repository contains **architecture code, preprocessing pipeline, and workflow documentation**.  
Due to dataset constraints, full training data is not included.
