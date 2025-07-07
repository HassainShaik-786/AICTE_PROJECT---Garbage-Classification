# AICTE_PROJECT --- Garbage - Classification using MobileNetV2

This project focuses on building an efficient image classification model to automatically classify garbage into six categories: `cardboard`, `glass`, `metal`, `paper`, `plastic`, and `trash`.

We utilized **MobileNetV2** as the backbone model through **transfer learning**, leveraging pre-trained weights from ImageNet to extract meaningful visual features. The workflow included:

- 📁 Custom dataset with 6 waste classes
- 🧹 Clean folder structure with `train`, `val`, and `test` splits
- 🖼️ Data augmentation to improve generalization
- 🔒 Initial training with frozen convolutional base
- 🧪 Validation monitoring using early stopping and learning rate reduction
- ✅ Fine-tuning the top layers of MobileNetV2
- 🎯 Label smoothing to reduce overconfidence and improve generalization
- 📊 Evaluation using classification report and confusion matrix
- 💾 Saved best-performing model after training (`garbage_classifier_final.h5`)

With this approach, the model achieved an accuracy of **82%**, demonstrating its potential in supporting automated waste segregation — a vital component in modern environmental and recycling systems.

### 📉 Why Not >90% Accuracy?
Despite rigorous training and evaluation, our model achieved a maximum accuracy of **86%** due to:
- Computational constraints limiting extended experimentation
