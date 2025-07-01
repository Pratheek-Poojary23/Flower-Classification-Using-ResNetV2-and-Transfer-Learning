# 🌸 Flower Classification Using ResNetV2 and Transfer Learning

A deep learning project that uses the ResNet50V2 architecture and transfer learning to classify images of flowers into multiple categories with high accuracy.

---

## 📌 Project Highlights

- ✅ **Architecture:** ResNet50V2 (pre-trained on ImageNet)
- ✅ **Technique:** Transfer Learning + Fine-Tuning
- ✅ **Dataset:** Flowers (Daisies, Dandelions, Roses, Sunflowers, Tulips)
- ✅ **Tools:** TensorFlow, Keras, OpenCV, NumPy, Matplotlib, Google Colab

---

## 📁 Directory Structure
```
├── ResNetV2_Transfer_Learning_for_Flower_Dataset.ipynb # Jupyter Notebook
├── dataset # flower data
```
---
## 🧠 Model Summary

The model is built using the **ResNet50V2** architecture pre-trained on ImageNet. Transfer learning is applied by freezing the convolutional base initially and then fine-tuning selected layers.

- **Base Model:** ResNet50V2 (include_top=False)
- **Input Shape:** 224 × 224 × 3
- **Transfer Learning:** Enabled (pre-trained on ImageNet)
- **Classifier Head:**
  - GlobalAveragePooling2D
  - Dense (Number of classes with softmax activation)
- **Loss Function:** Categorical Crossentropy
- **Optimizer:** Adam
- **Training Strategy:**
  - Freeze base model, train top layers
- **Epochs:** 5
- **Batch Size:** 32
---

## 📊 Evaluation Results

Performance of the trained model on the flower classification task:

| Dataset       | Accuracy     | Loss        |
|---------------|--------------|-------------|
| Training Set  | ~98%         | ~0.05       |
| Validation Set| ~86%         | ~0.15       |
| Test Set      | ~94–96%      | ~0.12       |


---

