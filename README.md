# 🌸 Flower Image Classification using CNN & TensorFlow

This deep learning project classifies flower images into five categories: **daisy, dandelion, rose, sunflower,** and **tulip**, using a Convolutional Neural Network (CNN) built with TensorFlow. The trained model is also deployed with an interactive interface using **Streamlit**.

---

## 📌 Objectives

- Build a CNN to classify flower species based on image input.
- Use data augmentation to improve generalization.
- Train, validate, and evaluate the model on a real-world image dataset.
- Deploy the model using **Streamlit** for easy image prediction.

---

## 🗂️ Dataset Overview

- **Total Images:** 4314  
- **Classes:** 5 (daisy, dandelion, rose, sunflower, tulip)  
- **Source:** Manually loaded from folders using `image_dataset_from_directory`

**Class Distribution:**
- daisy – 763
- dandelion – 1051
- rose – 783
- sunflower – 733
- tulip – 984

---

## 🧰 Tech Stack

- **Languages**: Python  
- **Libraries**: TensorFlow, Keras, NumPy, Matplotlib, Streamlit  
- **Model**: Convolutional Neural Network (CNN)  
- **Deployment**: Streamlit App

---

## 🧠 Model Architecture
Input (180x180x3)
→ Data Augmentation (Flip, Zoom, Rotate)
→ Rescaling Layer
→ Conv2D → MaxPooling
→ Conv2D → MaxPooling
→ Conv2D → MaxPooling
→ Dropout
→ Flatten
→ Dense (128 ReLU)
→ Dense (5 output logits)
Optimizer: Adam

Loss Function: SparseCategoricalCrossentropy (from_logits=True)

Accuracy Achieved: ~79.6% (Train), ~71.5% (Validation)

##  📈 Training Results
Epoch	Train Accuracy	Val Accuracy	Train Loss	Val Loss
1	35.8%	50.5%	1.52	1.21
8	70.7%	69.4%	0.73	0.83
15	79.6%	71.5%	0.52	0.76

##  🧪 Prediction Example
Image: Sample/dandelion.jpg.jpg
Output: 'The Image belongs to dandelion with a score of 91.13%'
🚀 Deployment with Streamlit
The trained model is deployed using Streamlit for browser-based interaction.

## Features:
1.Upload image via web interface

2.See live prediction output

3.View uploaded image preview

## Run Locally:
streamlit run app.py

## 🔎 Folder Structure

flower-classifier/
├── flowers/                   # Dataset folders
├── Flower_Recog_Model.keras   # Saved CNN model
├── app.py                     # Streamlit App
├── notebook.ipynb             # Training and EDA
├── upload/                    # Temp upload storage
└── README.md                  # Project Overview

## 📌 How to Use
1.Clone the repository

2.Ensure TensorFlow and Streamlit are installed

3.Run the model training script (or load the saved .keras file)

4.Launch the web app via Streamlit

## ✅ Key Learnings
1.Built and tuned a CNN for multi-class classification.

2.Applied data augmentation and prefetch caching to optimize training.

3.Successfully deployed the model using Streamlit for end-user interaction.

## 🙋‍♂️ Author
Nabeel Siddiqui
📧 nabeelsiddiqui468@gmail.com

## 📃 License
Open-source project licensed under MIT License.

---





