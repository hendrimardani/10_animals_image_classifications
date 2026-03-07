# Dataset Description

It contains about 28K medium quality animal images belonging to 10 categories: dog, cat, horse, spyder, butterfly, chicken, sheep, cow, squirrel, elephant.

# Project Description

This project was developed to build a highly accurate image classification model. The dataset consists of thousands of animal images across 10 classes: butterfly, cat, chicken, cow, dog, elephant, horse, sheep, spider, and squirrel.
The data processing pipeline includes custom image augmentation (rotation, flipping, brightness adjustment, blurring, and affine transformations) to enrich the dataset and prevent overfitting. Furthermore, the project utilizes **Transfer Learning** with the MobileNetV2 architecture to achieve maximum accuracy and faster convergence.

# Key Features

- **Data Augmentation:** Implemented custom augmentation techniques to improve model generalization.
  - Before Augmentation
  - After Augmentation

- **Transfer Learning:** Utilized the pre-trained MobileNetV2 model, which resulted in a high validation accuracy of over 94%.
- **TFLite Model Export:** Successfully converted the trained model into a `.tflite` format, facilitating efficient deployment on mobile and edge devices.

# Technologies & Libraries Used

- **Programming Language:** Python 3
- **ML Framework:** TensorFlow & Keras
- **Data Manipulation & Visualization:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Image, OpenCV
- **Deployment & Conversion:** TensorFlow.js / TensorFlow Lite

# Evaluation & Conclusion

The model demonstrated excellent image recognition performance:

- The evaluation metrics showed a high Validation Accuracy (~95%).
- The inference scripts (`infer_saved_model()` and `infer_tflite()`) successfully predicted the correct labels for the given test images.

# How to Use

1. Clone or download this repository.
2. Ensure your Python environment has the required libraries installed.
3. Open and run the Jupyter Notebook `image-classifications-animals-10.ipynb`.
4. You can use the generated `tflite_model.tflite` file located in the main directory to integrate the model into your applications (e.g., Android/iOS).
