#  Week 2 Report – Model Training (Garbage Classification)

## ✅ Objective
In Week 2, the goal is to build, compile, and train a convolutional neural network using **Transfer Learning** to classify garbage images into their respective categories.

---

## ⚙️ Tools & Libraries Used
- Python 3.x  
- TensorFlow / Keras  
- NumPy, Matplotlib  
- Pretrained model: **MobileNetV2**

---

## 🏗️ Model Architecture

- **Base Model:** MobileNetV2 (pretrained on ImageNet, include_top=False)
- **Custom Top Layers:**
  - GlobalAveragePooling2D
  - Dense (ReLU)
  - Dropout for regularization
  - Output Layer with Softmax activation (multi-class classification)

---

## 🔧 Steps Performed

1. **Loaded MobileNetV2** without top layers to use as a feature extractor
2. **Added custom dense layers** on top for classification
3. **Froze the base model** to retain pretrained weights
4. **Compiled the model** with:
   - Optimizer: `Adam`
   - Loss: `categorical_crossentropy`
   - Metric: `accuracy`
5. **Trained the model** on the augmented dataset for several epochs
6. **Saved the trained model** for future evaluation

---

## 📊 Results & Metrics

- Model trained for X epochs  
- Achieved ~XX% accuracy on validation data  
- Loss and accuracy curves show stable learning

---

## 📈 Visualizations
- Plotted training vs validation accuracy and loss
- Verified model convergence and checked for overfitting

---

## ✅ Deliverables

- ✅ `model_training.ipynb` notebook  
- ✅ Saved trained model (`garbage_classifier.h5`)  
- ✅ Accuracy/loss plots  
- ✅ Updated directory structure

