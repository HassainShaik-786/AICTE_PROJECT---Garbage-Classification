# 🗑️ Week 1 Report – Garbage Classification Project

## ✅ Objective

The goal of Week 1 is to set up the dataset and apply preprocessing steps to prepare garbage images for model training using transfer learning.

---

## 📁 Dataset

The dataset contains images of garbage categorized into classes:
- Cardboard
- Glass
- Metal
- Paper
- Plastic
- Trash

Each class has a separate folder of images. This classification helps automate waste sorting and supports recycling systems.

---

## ⚙️ Tools & Libraries

- Python 3.x  
- TensorFlow / Keras  
- NumPy  
- Matplotlib  
- Google Colab / Jupyter Notebook  

---

## 🔧 Preprocessing Steps

1. **Load the Dataset**
   - Used `ImageDataGenerator.flow_from_directory()` to load images efficiently.

2. **Image Resizing**
   - All images resized to `224x224` to match MobileNetV2 input size.

3. **Normalization**
   - Pixel values scaled to range `[0, 1]`.

4. **Data Augmentation**
   - Applied real-time transformations:
     - Rotation
     - Horizontal flip
     - Zoom
     - Brightness adjustment

5. **Train-Validation-Test Split**
   - Split dataset into:
     - 70% training
     - 15% validation
     - 15% test

---

## 📁 Folder Structure

