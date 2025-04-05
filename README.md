#  Skin Cancer Classification using Deep Learning  
### Group 15 – University of Calgary | ENEL 645 - Data Mining and Machine Learning.

---

##  Project Overview  
This project presents a deep learning pipeline to classify skin cancer lesions as **benign** or **malignant** using dermoscopic images. We trained and evaluated five different convolutional neural network (CNN) models to compare their effectiveness in detecting melanoma from images.

###  Models Used:
-  Custom CNN  
-  ResNet50V2  
-  EfficientNetB2  
-  EfficientNetB3  
-  EfficientNetB4  

Each model was trained using a preprocessed dataset with balanced classes and augmented images to improve generalization.

---

##  Dataset  
- **Source:** [Melanoma Skin Cancer Dataset (Kaggle)](https://www.kaggle.com/datasets/hasnainjaved/melanoma-skin-cancer-dataset-of-10000-images)  
- **Total Images:** 10,605  
  - Training: 9605  
  - Testing: 1000  
- **Classes:**
  - 0 = Benign  
  - 1 = Malignant  

###  Preprocessing:
- Resized images based on model requirements (224x224 to 380x380)  
- Normalized pixel values to [0, 1]  
- Applied data augmentation (flip, rotate, zoom, brightness)  
- Used class weights to handle data imbalance

---

##  Training Details
- **Epochs:** 10  
- **Batch Size:** 32  
- **Optimizer:** Adam with learning rate decay  
- **Loss Function:** Binary Crossentropy  
- **Callbacks:** EarlyStopping, ModelCheckpoint  
- **Validation Split:** 10% from training data

---

##  Evaluation Metrics
The models were evaluated using the following metrics:
- Accuracy  
- Precision  
- Recall  
- F1-Score  
- Confusion Matrix  
- ROC AUC Curve  


>  **Best Validation Accuracy:** ResNet50V2 with 91.5%  
>  **EfficientNetB2 Misclassified Samples:** 332/1000

---

##  Visual Outputs
- Accuracy/Loss plots for each model  
- Confusion Matrix  
- ROC Curves  
- Misclassified image visualizations with predicted and true labels

---

##  Run the Project
**Google Colab Notebook:**  
[Open in Colab](https://colab.research.google.com/drive/10XUhDIofvWu0nTNowdLhkHIPzL3AGQQj)

---

##  Group Members – Group 15

| Name               | Student ID |
|--------------------|------------|
| Om Vipulbhai Patel | 30243246   |
| Sanket Patel       | 30246586   |
| Sadia Khan         | 30090271   |
| Ramanpreet Kaur    | 30270427   |

---



