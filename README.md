<h1 align="center">Floralytics</h1>
This CNN-based flower classification model processes the Flowers Recognition dataset, utilizing image augmentation and deep learning to classify Daisy, Dandelion, Rose, Sunflower, and Tulip. The model achieves 97% accuracy with optimized convolutional layers ensuring robust feature extraction and high-performance classification.

## Execution Guide:
1. Run the following command line in the terminal:
   ```
   pip install tensorflow keras numpy pandas matplotlib seaborn scikit-learn opencv-python pillow
   ```

2. Download the dataset (link to the dataset: https://www.kaggle.com/datasets/alxmamaev/flowers-recognition)

3. Copy and paste the path of the images into the code

4. Upon running the code the model outputs its prediction

## Model Prediction:

![image](https://github.com/user-attachments/assets/f5ae4c6b-c90a-4a52-b9ba-62a43411db34)

![image](https://github.com/user-attachments/assets/2f24ebf3-f48e-4670-acf9-6d12e8df291f)

![image](https://github.com/user-attachments/assets/88d66c29-ab76-4d64-b82f-3dc6c3c5477c)

![image](https://github.com/user-attachments/assets/c01e0bac-ba7f-4af4-9b50-78c68cc3c9fd)

![image](https://github.com/user-attachments/assets/dddbf1a2-c9ee-4c5a-8502-6c5cd05f67d3)

## Accuracy & Loss over Epochs:

![image](https://github.com/user-attachments/assets/6cad210d-4e2e-4fba-8f6b-3a5325e3760b)

![image](https://github.com/user-attachments/assets/524bf426-4d2b-474c-b0bf-61abdc9b117c)

## Overview:
The system is a deep learning-based image classification model that identifies different types of flowers using a convolutional neural network (CNN). Here’s an overview of the process:

### **1. Importing Required Libraries**  
Essential Python libraries such as TensorFlow, OpenCV, NumPy, Pandas, and Matplotlib are imported for image processing, model building, and visualization.

### **2. Dataset Preparation**  
- The **Flowers Recognition** dataset from Kaggle is downloaded and extracted.  
- Data is preprocessed using **ImageDataGenerator** for augmentation and normalization.  
- Training and validation datasets are split with an 80-20 ratio.

### **3. Model Architecture**  
- A **CNN** is built with multiple convolutional and max-pooling layers.  
- The final layers include a **Flatten**, **Dense (512 neurons with ReLU activation)**, and an **output layer (softmax for 5 classes: daisy, dandelion, rose, sunflower, tulip)**.

### **4. Model Compilation & Training**  
- The model is compiled using the **Adam optimizer** with **categorical cross-entropy loss**.  
- Training is performed for **30 epochs**, showing gradual improvements in accuracy.  
- Accuracy increases significantly but validation accuracy fluctuates.

### **5. Model Evaluation**  
- The trained model is tested on the validation dataset.  
- The **accuracy is calculated**, and a **classification report & confusion matrix** are generated.  
- Training accuracy is high, but validation accuracy is lower, indicating possible **overfitting**.

### **6. Visualizing Performance**  
Plots for **accuracy & loss over epochs** help analyze training behavior.

### **7. Making Predictions**  
- A function is created to load an image, preprocess it, and predict the flower class.  
- Predictions are displayed with **confidence scores** and the corresponding image.
