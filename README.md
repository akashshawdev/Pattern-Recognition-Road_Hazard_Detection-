# 🛣️ Road Hazard Detection System
### *Automated Detection & Severity Classification of Cracks & Potholes*

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-red.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-4.0+-green.svg)
![License](https://img.shields.io/badge/License-Academic-yellow.svg)

**Module:** PW25 - SE01 Pattern Recognition (60 + 90 + 120)  
**Professor:** Dr. Raja Hashim Ali  
**Group:** WS25-PR7

</div>

---

## 👥 Team Members

| Name | Role | Responsibilities |
|------|------|-----------------|
| **Syed Muhammad Huzaifa Ali** | 🔧 Technical Lead | Model Architecture, Code Implementation, System Integration |
| **Akash Kumar Shaw** | 📊 Figures & Presentation | Data Visualization, Performance Analysis, Presentation Design |
| **Ishtpreet Singh** | 📝 Final Report Writing & Submission | Documentation, Report Compilation, Project Submission |

---

## 📋 Project Overview

This project presents an **intelligent Road Hazard Detection System** that automates road surface inspections using advanced deep learning techniques. By combining a **Convolutional Neural Network (CNN)** with a **Rule-Based Meta-Learner**, our system goes beyond simple detection—it evaluates hazard severity to help civil engineers prioritize maintenance and repairs effectively.

### 🎯 Key Features

- 🧠 **Deep Learning Classification:** ResNet-18 based CNN for pattern recognition
- 📏 **Geometric Analysis:** OpenCV-powered dimension measurement
- ⚖️ **Severity Assessment:** Intelligent rule engine for maintenance prioritization
- 📊 **Comprehensive Reporting:** Automated CSV generation with actionable insights
- 🔄 **Real-time Validation:** Epoch-by-epoch performance tracking

---

## 🗂️ Dataset Information

We utilize the **RDD-2022 (China_Urban subset)** dataset for training and evaluation.

### 📥 Dataset Setup

1. **Download:** Get the dataset from [Kaggle - RDD-2022](https://www.kaggle.com/datasets/aliabdelmenam/rdd-2022/data)
2. **Rename:** Change the downloaded file from `archive.zip` to `rdd-2022.zip`
3. **Upload:** Place `rdd-2022.zip` in the **root directory** of your Google Drive
4. **Process:** Our automated pipeline handles extraction and preprocessing

> ⚠️ **Important:** Ensure the file is named exactly `rdd-2022.zip` and placed in `MyDrive` root for proper synchronization.

---

## 🏗️ Technical Architecture

Our system employs a sophisticated three-tier architecture:

### 1️⃣ **The Brain - CNN Classifier**
- **Model:** ResNet-18 (Pre-trained on ImageNet)
- **Classes:** Normal, Crack, Pothole
- **Output:** Classification confidence scores

### 2️⃣ **The Measurement - Meta-Learner**
- **Technology:** OpenCV contour analysis
- **Metrics:** Area (pixels), Aspect Ratio
- **Purpose:** Physical dimension quantification

### 3️⃣ **The Decision - Rule Engine**
- **Logic:** Fusion of CNN confidence + geometric features
- **Example:** Potholes > 5,000 pixels → Classified as "Severe"
- **Benefit:** Context-aware severity assessment

---

## 🚀 How to Reproduce

### Prerequisites
- Google Account with Drive access
- Google Colab (free tier sufficient)
- Basic understanding of Python and Jupyter notebooks

### Step-by-Step Instructions

```bash
# 1. Prepare Dataset
# Download rdd-2022.zip from Kaggle
# Rename to: rdd-2022.zip
# Upload to: Google Drive root (/MyDrive/)

# 2. Open Notebook
# File: Road_Hazard_Detection_Technical_Lead(S.M. Huzaifa Ali).ipynb
# Platform: Google Colab

# 3. Mount Google Drive
# Run the initialization cells in the notebook
# Default path: /content/drive/MyDrive/rdd-2022.zip

# 4. Execute Pipeline
# Training: Run Cell 7 (10 epochs with validation)
# Evaluation: Run Cell 8 (Confusion matrix & metrics)
# Inference: Run Cell 12 (Batch processing & CSV export)
```

### 📁 Notebook Structure

| Cell | Function | Description |
|------|----------|-------------|
| 1-3 | 🔧 Setup | Drive mounting, dependency installation |
| 4-5 | 📦 Data Prep | Extraction, path synchronization, cropping |
| 6 | 🏗️ Model Build | ResNet-18 initialization, transfer learning |
| 7 | 🎓 Training | 10-epoch training with validation tracking |
| 8 | 📊 Evaluation | Performance metrics, confusion matrix |
| 9-11 | 🔍 Analysis | Meta-learning integration, severity logic |
| 12 | 📤 Export | Batch inference, CSV report generation |

---

## 🔬 Research Questions & Outcomes

### ✅ RQ1-3: Model Performance
- Established **baseline accuracy** on China_Urban dataset
- Achieved strong **regional generalization**
- Validated **transfer learning effectiveness** with ResNet-18

### ✅ RQ4: Visual Analysis
- Generated comprehensive **confusion matrices**
- Demonstrated **high precision** in hazard detection
- Identified model strengths and improvement areas

### ✅ RQ5: Maintenance Intelligence
- Successfully distinguished **cosmetic cracks** from **critical potholes**
- Implemented **severity classification** for prioritization
- Enabled **data-driven maintenance** decision-making

---

## 📊 Expected Results

### Model Metrics
- 🎯 **Accuracy:** Competitive performance on test set
- 📈 **Precision/Recall:** Balanced detection capabilities
- 🔥 **Confusion Matrix:** Clear visualization of predictions

### Output Deliverables
- 📄 **CSV Report:** Detailed hazard inventory with severity levels
- 📉 **Training Curves:** Loss and accuracy progression graphs
- 🗺️ **Visual Predictions:** Annotated images with bounding boxes

---

## 🛠️ Technologies Used

<div align="center">

| Category | Tools |
|----------|-------|
| **Deep Learning** | PyTorch, ResNet-18, Transfer Learning |
| **Computer Vision** | OpenCV, PIL, Image Preprocessing |
| **Data Science** | NumPy, Pandas, Matplotlib, Seaborn |
| **Development** | Python 3.8+, Jupyter Notebooks, Google Colab |
| **Storage** | Google Drive API, Cloud Integration |

</div>

---

## 📝 Citation

If you use this project in your research or work, please cite:

```bibtex
@project{road_hazard_detection_2025,
  title={Road Hazard Detection System: Automated Crack and Pothole Classification},
  author={Ali, Syed Muhammad Huzaifa and Shaw, Akash Kumar and Singh, Ishtpreet},
  year={2025},
  institution={Pattern Recognition - PW25 SE01},
  supervisor={Dr. Raja Hashim Ali}
}
```

---

## 📧 Contact

For questions, suggestions, or collaboration opportunities:

- **Technical Lead:** Syed Muhammad Huzaifa Ali
- **Module:** PW25 - SE01 Pattern Recognition
- **Group:** WS25-PR7

---

## 📜 License

This project is developed for **academic purposes** as part of the Pattern Recognition course. All rights reserved by the team members and the academic institution.

---

<div align="center">

### 🌟 Built with passion for safer roads 🌟

**Made with ❤️ by Team WS25-PR7**

</div>
