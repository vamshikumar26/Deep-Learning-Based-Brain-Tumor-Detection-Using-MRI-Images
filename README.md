# Brain Tumor Detection Using Deep Learning

This project implements an **AI-based system to detect brain tumors** from MRI images using deep learning (CNNs). A trained model is integrated with a **Flask-based web interface** where users (e.g., doctors) can upload brain scan images to get instant predictions.

---

## Objective

To assist healthcare professionals in early detection of brain tumors by automating the diagnosis process through image classification using deep learning.

---

## Model Overview

- **Architecture**: Convolutional Neural Network (CNN)
- **Dataset**: MRI images (~3000 labeled samples)
- **Training**: Done in `brain-tumor-detection.ipynb`
- **Deployment**: Web app built using **Flask**

---

## Project Structure

brain-tumor-detection/
├── dataset/ # Contains training/test MRI images

├── pages/ # HTML pages for Flask frontend

│ ├── index.html

│ └── predict.html

├── pretrain_model/ # Directory where trained model weights are stored

│ └── model.h5

├── main.py # Flask app entry point for image upload and prediction

├── brain-tumor-detection.ipynb # Jupyter notebook for training the model

├── requirements.txt # Project dependencies

└── README.md


---

##  Setup Instructions

### Clone the Repository

git clone https://github.com/yourusername/brain-tumor-detection.git
cd brain-tumor-detection

## Install Dependencies

pip install -r requirements.txt

## Run the Flask App
python main.py

## Open in Browser
Go to http://127.0.0.1:5000/ and upload an MRI image to detect if a tumor is present.

# Dataset Info
MRI scans labeled as tumor and no tumor

Size: ~3000 images

Used for binary image classification

## Model Training
The CNN model was trained in the provided Jupyter Notebook:

Preprocessing: Image resizing, normalization

Data Augmentation: To improve generalization

Model saved to: pretrain_model/model.h5

## Web Interface Preview
Upload brain MRI scans

Instant tumor detection result with UI feedback

## Use Cases
Assisting radiologists and doctors in tumor detection

Reducing manual screening time

Supporting early-stage diagnosis

## Screenshots
<center><img src="Brain Tumor Prediction - Personal - Microsoft​ Edge 29-01-2023 20_32_24.png"></center>
