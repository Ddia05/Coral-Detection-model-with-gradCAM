# Coral Bleaching Detection with Explainable AI

A deep learning system that detects coral bleaching severity from underwater images and explains predictions using Grad-CAM visualizations.

![Screenshot 2025-07-06 171332](https://github.com/user-attachments/assets/08ecbb94-007a-4f5e-90dc-522a617fdd74)
![image](https://github.com/user-attachments/assets/e5b4b267-d27e-4065-b445-6084ad77633e)

---

## Project Overview

This project aims to support marine conservation efforts by providing an AI-driven tool that:
- Classifies the **severity of coral bleaching on a scale from 1 to 10**
- Generates **Grad-CAM heatmaps** to visually explain model decisions
- Provides an **interactive Gradio web interface** for real-time testing

All training and inference is done entirely in **Google Colab**, avoiding the need to install heavy libraries or use local compute.
---

## Features

- ResNet18-based classifier trained on a **custom-labeled dataset** of coral images
- Explainability with **Grad-CAM** to highlight regions influencing predictions
- **Gradio interface** for easy image upload and visualization
- Model performance improves with custom label cleaning and balanced training
- Cloud-based: runs entirely on **Google Colab**

---

## Directory Structure
coral_detection_model/

│

├── All_Images/ # Coral images (img1.png to img342.png)

├── labels.csv # CSV with image filenames and bleaching scores

├── coral_classifier.ipynb # Colab notebook for training and prediction

└── README.md # Project readme

---

## Tech Stack

- **Python**
- **PyTorch**
- **ResNet18 (pretrained)**
- **Grad-CAM**
- **Gradio**
- **Google Colab**

---

## Example Usage

Upload a coral image via the Gradio interface. The model returns:
- **Predicted bleaching score** (0 to 10)
- The **original image**
- A **Grad-CAM heatmap**
- An **overlay** of the heatmap on the original image
Example image provided at the beginning 

---

This project contributes to **sustainable ocean monitoring** by enabling scalable, explainable AI analysis of coral health, supporting **UN Sustainable Development Goal 14: Life Below Water**.

---

## Acknowledgements

- Pretrained ResNet18 model from `torchvision`
- Grad-CAM methodology from open-source implementations

---

## Contact

Feel free to connect for questions or improvements
